# 📅 Linux Basics Day2
---
## Linux Commands Learned Today

- **whoami** - Its a fun command that can tell you who you are logged in as.
- **sudo** - Its an essential command that is needed to run administrator commands.
- **adduser** - Its an admin command which can add another user to the system. We need to use "sudo" to run this command.
    **Ex-** `sudo adduser USER1`
- **which** - This command is used to know the location of where your running commands are stored.
    **Ex-** which ls
It will give you location of where `ls` command is stored.
- **touch** - This command is used to create files in a directory.
    **Ex-** `touch textfile.txt`
- **nano** - This command is used to enter the data in the created file.
   + To save: CTRL + O → press Enter
   + To exit: CTRL + X
- **mv** - This command is used to move the file from one directory to another.
	**Ex-** `mv testfile.txt /home/user/test`
Here "testfile.txt" which was initially stored in another directory will be moved to "/home/user/test" directory.
- **find** - This command is most useful as it can help u find different files on basis of different conditions. Such as-
	+ **By Name** - ind /path/ -name = This condition finds file on the basis of name entered. It is case sensitive.
	   **Ex-** `find . -name test`
	   Here "." represents current directory and "test" is the name of file.
	+ **By name (case-sensitive)** - find /path/ iname- = It is same as name but it ignore case sensitive searches.
	+ **By Size** - find /path/ -size = It helps in finding a file based on certain size. Here M represents MB, k represents KB, G represents GB, c represents bytes
	   **Ex-** `find . -size 50M`
	   Here "50M" represents 50MB size of file.
	+ **By Type** - find /path/ -type = It helps in finding a file based on type. Here f for file, d for directory, l for symbolic link, b for block device, s for socket.
	+ **By User** - find /path/ -user = This commands helps in selecting file of a particular user only.

## Bandit Progress

+ **level 2-** Learnt how to read a file which has '-' as its name.
+ **level 3-** Learnt how to read a file which has spaces in  its name.
+ **level 4-** Learnt how to locate and read a hidden file.

## Things That Amazed Me

It was very surprising to know that everything we have whether its linux commands, hard disks, virtual disks or even our devices that we can mount in our system. IT'S ALL A FILE!!!
Literally everything is a file and since its a file we can even delete, edit, modify or change it. Although its quite a hard task to do as everything written in these files are in binary language.

## Most Useful Command I Found Today

**find** – It’s an extremely helpful command that can locate files by name, type, size, or ownership. Just a small command, and it finds exactly what you're looking for — making it incredibly powerful for cybersecurity, scripting, and system administration.