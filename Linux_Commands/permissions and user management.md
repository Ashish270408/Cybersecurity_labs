# 🔐 Permissions & Ownership

- **chmod** - This command is used to edit permissions in a file.  
	**Ex-** `chmod a+rwx files.txt`  
Here, `a` means for all, `+` means to add, `rwx` are permissions.  
In the same case, we can use `u` for user, `g` for group, `o` for other instead of `a` as per our convenience.  
To edit permission of entire directory we can use this-  
	**Ex-** `chmod -R u=rwx testdir/`
- **chown** - It can be used to change ownership of a specific file.  
	**Ex-** `chown paul:root test.txt`  
Here ownership of `test.txt` will be given to `paul`.
- **chgrp** - It can be used to change group of a file.  
	**Ex-** `chgrp paul test.txt`

# 👤 User Management & Privileges

- **whoami** - Its a fun command that tells you who you are logged in as.
- **sudo** - Its a essential command that is needed to run administrator commands.
- **adduser** - Its an admin command which can add another user to the system. We need to use sudo to run this command.  
	**Ex-** `sudo adduser USER1`
- **which** - This command is used to know the location of where your running commands are stored.  
	**Ex-** `which ls`  
It will give you location of ls command where it is stored.