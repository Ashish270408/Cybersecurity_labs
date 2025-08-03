# 🧹 Text Processing

- **cut** - This is used to  pick a specific word from a line.  
	**Ex-** `cut -d " " -f 12`  
Here `-d` is a delimiter which says to cut each string after ` `(space)
- **sort** - It sorts all the filtered results alphabetically
- **uniq** - It will display only unique records removing any duplicates.  
If it is used with flag `-d`, it will give unique entries of those which have duplicate entries.  
And if used with `-u`, it will give only those entries which appeared only once.
- **'>'** - This arrow syntax can be used to save the data we have filtered from to a certain file in certain location.  
	**Ex-** `cat trial.txt | grep "Hello" > ~/Hello.txt`  
This will save all the lines that contain `Hello` in `~/` directory with name `Hello.txt`.
- **wc** - It is used for word count and can be used in following ways-
    + wc -l 
    + wc -c 
    + wc -w  
Where, `-l` counts lines, `-c` counts bytes and `-w` counts words.