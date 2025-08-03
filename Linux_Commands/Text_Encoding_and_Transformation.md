# 🔡 Text Encoding & Transformation

- **strings** - It is one of the most useful commands as it helps you filter out human readable words from binary junks.  
	**Ex-** `strings data.txt`  
It can be used with `-n` flag which will help you filter words which have at least selected number of characters.  
	**Ex-** `strings -n 4 data.txt`   
It will filter only those human readable words which are at least 4 characters long.
- **base64** - Its a format of encoding a string in such a way so that data is not lost.  
We can decode this coded data with the help of `base64 --decode` command.  
	**Ex-** `echo 'Hello' | base64`  
This will encode the data, say `SGVsbG8K`. Now to decode it we can use-  
	**Ex-** `echo "SGVsbG8K" | base64 --decode`
- **tr** - This command is used to transform lowercase to uppercase and vice versa.  
	**Ex-** `echo "Hello World" | tr [a-z] [A-Z]`  
This command will convert all lowercase `[a-z]` to uppercase `[A-Z]` which will print `HELLO WORLD`.  
We can also delete the specific case letters with it using `-d` flag.  
	**Ex-** `echo "Hello World" | tr -d [a-z]`  
This will delete all the lowercase letter and output will be `H W`.  
We can also delete duplicate letters using `-s` flag.  
	**Ex-** `echo "Hello World" | tr -s "l"`  
Output will be `Helo World`  
We can use it to delete any specific characters as well using `-d` flag and also replace a character with something else in this way-  
	**Ex-** `echo "Hello World" | tr "l" "o"`  
	**Output-** `Heooo Worod`
- **ROT13** - Its an old way of encrypting data which changes a letter to the next 13th letter to it. It can be done with `tr` in this way-  
	**Ex-** `echo "Hello World" | tr 'A-Za-z' N-ZA-Mn-za-m'`  
Repeating it will decode the sentence.