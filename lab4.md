# Lab 4
## Linux CLI ( Command Line Interface )
[![Linux](https://softwarelab.org/wp-content/uploads/Linux.jpg)](https://linuxcommand.org)
### Shell command

- `pwd`

shows the current path in a hierarchical directory
```
$ pwd
/home/<username>
```

---
- `cd`

change directory
```
$ cd Desktop
~/Desktop $
```

---
- arguments
  
  * /   
  root
  
  * .   
  current directory
  
  * ..   
  upper-level directory
  
  * ~   
  home of current user
  
  * /   
  absolute path
  
  * ./   
  relative path
  
  * ../   
  relative path

---
- options

  * -l   
  show detailed information(long format)

  * -lh   
  same as above, but size in units

---
- `ls`

list files and directories   

>`ls /bin`   
List the files in the /bin directory (or any other directory we care to specify)

>`ls -l`   
List the files in the working directory in long format   
```
$ls -l
-rw--------------  1me       me        34653          Sep 21 2023         README.md

-----------------  -------  --------- --------------  -----------------  -----------
File permissions   Owner    Group     Size(in bytes)  Modification Time  File Name
```

>`ls -l /etc /bin`   
List the files in the /bin directory and the /etc directory in long format

>`ls -la ..`   
List all files ( even ones with names beginning with a period character, which are normally  hidden ) in the parent of the working directory in long format   

```
$ ls
<file 1> <file 2> <file 3> <folder 1> <folder 2> <folder 3>
```

---
- `cp`

copy files and directories

>`cp file1 file2`   
Copies the contents of file1 into file2. If file2 does not exist, it is created; otherwise, file2 is silently overwritten with the contents of file1.

>`cp -i file1 file2`   
Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.

>`cp file1 dir1`   
Copy the contents of file1 (into a file named file1) inside of directory dir1.

>`cp -R dir1 dir2`   
Copy the contents of the directory dr1. If directory dir2 does not exist, it is created, Otherwise, it creates a directory names dir1 within directory dir2.

```
$ cp a.py b.py
$ ls
a.py b.py
```

---
- `mv`

move files and directories or rename them

>`mv file1 file2`   
If file2 does not exist, then file1 is renamed file2. If file2 exists, its contents are silently replaced with the contents of file1.

>`mv -i file1 file2`   
Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1

>`mv file1 file2 dir1`   
The files file1 and file2 are moved to directory dir1. If dir1 does not exist, mv will exit with an error.

>`mv dir1 dir2`   
If dir2 does not exist, then dir1 is renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2.

```
$ ls
a.py
$ mv a.py b.py
% ls
b.py
```

---
- `rm`

delete files and directories permantely and irreversevely

>`rm file1 file2`   
Delete file1 and file2

>`rm -i file1 file2`   
Like above however, since the "-i" (interactive) option is specified, the user is prompted before each file is deleted.

>`rm -r dir1 dir2`   
Directories dir1 and dir2 are deleted along with all of their contents.

```
$ ls
a.py
$ rm a.py
$ ls

```

---
- `mkdir`

make a new directory
```
$ mkdir folder
$ls
folder
```

---
- Wildcards

  * \*    
  All filenames
  
  * g*   
  All filenames that begin with the character "g"
  
  * b*.txt   
  All filenames that begin with the character "b" and with the characters ".txt"
  
  * Data???   
  Any filename that begins with the characters "Data" followed by exactly 3 more characters

---
- `help`

```
$ help <command>
<explain about command>
```

---
- `man`

```
$ man <command>
<explain about manual of command>
```

---
- `exit`

exiting terminal

