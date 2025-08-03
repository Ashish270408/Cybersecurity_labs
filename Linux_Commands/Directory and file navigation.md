# 📁 Directory & File Navigation

- **pwd (Print Working Directory) -** It tells you which directory you are working in.
- **ls -** It lists the contents of current directory.
- **ls -l (ll) -** This command is used to know information about the files.
- **ls -a -** This command shows all hidden and non-hidden files.
clear - Can be used to clear previous outputs on the terminal. It will provide you with fresh terminal page where you can carry on your task.
- **cd -** This command is used to navigate between directories and folders.
- **cd .. -** This command can take u back to previous directory.
- **cd / -** It is used to take you back to root directory (Initial or Main directory).
- **mkdir -** It is used to create a new directory.  
	**Ex-** `mkdir NEWFOLDER`
- **rmdir -** It is used to remove a directory. (!!!Can not delete directory if it has something stored in it!!!).  
	**Ex-** `rmdir NEWFOLDER`
- **find -** This command is most useful as it can help u find different files on basis of different conditions. Such as-
	+ **find /path/ -name =** This condition finds file on the basis of name entered. It is case sensitive.  
	   **Ex-** `find . -name test`
	   Here "." represents current directory and "test" is the name of file.  
	+ **find /path/ iname- =** It is same as name but it ignore case sensitive searches.
	+ **find /path/ -size =** It helps in finding a file based on certain size. Here M represents MB, k represents KB, G represents GB, c represents bytes.  
	   **Ex-** `find . -size 50M`
	   Here "50M" represents 50MB size of file.
	+ **find /path/ -type =** It helps in finding a file based on type. Here f for file, d for directory, l for symbolic link, b for block device, s for socket.
	+ **find /path/ -user =** This commands helps in selecting file of a particular user only.
	+ **find /path/ -group =** This command helps in selecting file of a particular group only.