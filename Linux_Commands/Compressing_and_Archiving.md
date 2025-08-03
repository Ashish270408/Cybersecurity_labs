# 🧳 Compression & Archiving

- **xxd** - It is used for hexadump encryption. It can convert data into hexadecimal.  
	**Ex-** `xxd data.txt`  
To decrypt it we can use `-r` flag with xxd.  
	**Ex-** `xxd -r data.txt`
- **gzip** - Its a way of compressing a file. It is fastest and compresses moderately. Extension of file is `.gz`.  
To decompress this file one can use `gunzip data.gz`
- **bzip2** - It's another way of compressing data which is slower then gzip but better. Its extension is `.bz2`.  
To decompress one can use `bunzip2 data.bz2`.
- **xz** - It is also another way of compressing data which is slowest of all but compresses file the most. Its extension is `.xz`.  
To decompress one can use `unxz data.xz`.
- **tar** - It is not a compressing but bundling the files. It can be done with the help of certain flags which are as follows-  
	+ **-c** = To create a tar file
	+ **-f** = to tell file name
	+ **-v** = To tell what is going on backscreen after running this cmd.
	+ **-x** = To unbundle the file
	+ **-z** = It bundles the file as well as compresses them to gzip.
	+ **-j** = It bundles the file as well as compresses them to bzip2.
	+ **-J** = It bundles the file as well as compresses them to xz.
	+ **-t** = It tells what files does tar holds without extracting them.  
	**Ex-** `tar -cf archive.tar data.txt file.txt`, `tar -xf archive.tar` etc.  
These flags are used with single `-` as in above examples. They can include more flags at once as per requirement.