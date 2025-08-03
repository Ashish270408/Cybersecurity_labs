# 🔎 Searching & Filtering

- **find** - This command is most useful as it can help u find different files on basis of different conditions. Such as-
	+ **By Name** - ind /path/ -name = This condition finds file on the basis of name entered. It is case sensitive.  
	   **Ex-** `find . -name test`  
	   Here `.` represents current directory and `test` is the name of file.
	+ **By name (case-sensitive)** - find /path/ iname- = It is same as name but it ignore case sensitive searches.
	+ **By Size** - find /path/ -size = It helps in finding a file based on certain size. Here `M` represents MB, `k` represents KB, `G` represents GB, `c` represents bytes.  
	   **Ex-** `find . -size 50M`  
	   Here `50M` represents 50MB size of file.
	+ **By Type** - find /path/ -type = It helps in finding a file based on type. Here f for file, d for directory, l for symbolic link, b for block device, s for socket.
	+ **By User** - find /path/ -user = This commands helps in selecting file of a particular user only.
- **grep** - It filters the files as per particular word.  
	**Ex-** `cat trial.txt | grep "Hello"`  
if it is used with flag `-v` then it will remove the lines that contain certain words and show the rest.  
	**Ex-** `cat trial.txt | grep -v "User"`  
Now all the lines which have "User" in it will be removed and rest will be shown.  
Here, `cat trial.txt` will read content of file, `|` is called pipe and it continues the previous command to `grep` which filters the content with specific word only.