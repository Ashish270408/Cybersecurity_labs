# 📅 Linux Basics Day4
---
## Linux Commands Learned Today

- **grep** - It filters the files as per particular word.  
	**Ex-** `cat trial.txt | grep "Hello"`  
if it is used with flag '-v' then it will remove the lines that contain certain words and show the rest.  
	**Ex-** `cat trial.txt | grep -v "User"`  
Now all the lines which have "User" in it will be removed and rest will be shown.  
Here, "cat trial.txt" will read content of file, '|' is called pipe and it continues the previous command to 'grep' which filters the content with specific word only.
- **cut** - This is used to  pick a specific word from a line.  
	**Ex-** `cut -d " " -f 12`  
Here `-d` is a delimiter which says to cut each string after `" "`space.
- **sort** - It sorts all the filtered results alphabetically
- **uniq** - It will display only unique records removing any duplicates.  
If it is used with flag `-d`, it will give unique entries of those which have duplicate entries.  
And if used with `-u`, it will give only those entries which appeared only once.
- **'>'** - This arrow syntax can be used to save the data we have filtered from to a certain file in certain location.  
	**Ex-** `cat trial.txt | grep "Hello" > ~/Hello.txt`  
This will save all the lines that contain "Hello" in `~/` directory with name `Hello.txt`.
- **wc** - It is used for word count and can be used in following ways-
    + wc -l 
    + wc -c 
    + wc -w  
Where, `-l` counts lines, `-c` counts bytes and `-w` counts words.
- **strings** - It is one of the most useful commands as it helps you filter out human readable words from binary junks.  
	**Ex-** `strings data.txt`  
It can be used with `-n` flag which will help you filter words which have at least selected number of characters.  
	**Ex-** `strings -n 4 data.txt`  
It will filter only those human readable words which are at least 4 characters long.
- **base64** - Its a format of encoding a string in such a way so that data is not lost.  
We can decode this coded data with the help of `base64 --decode` command.  
	**Ex-** `echo 'Hello' | base64`  
This will encode the data, say `SGVsbG8K`. Now to decode it we can use-  
	**Ex-** `echo 'SGVsbG8K' | base64 --decode`

## Bandit Progress

+ **level 7-** Learnt how to find a line with specific word.
+ **level 8-** Learnt how to fnd unique lines.
+ **level 9-** Learnt how to find human readable text in binary data.
+ **level 10-** Learnt how to encode and decode data using base64.

## Most Useful Command I Found Today

**Strings**- It can help you distinguish huamn readable data from binary data, which is quite fascinating and useful especiaally in cybersecurity.
