# Lab 4
## Linux CLI ( Command Line Interface )

### Shell command

- pwd

shows the current path in a hierarchical directory
```bash
$ pwd
/home/<username>
```

- cd

change directory
```
$ cd Desktop
~/Desktop $
```

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

- options

  * -l   
  show detailed information(long format)

  * -lh   
  same as above, but size in units

- ls

list files and directories   
**more**
>ls /bin   
List the files in the /bin directory (or any other directory we care to specify)

>ls -l   
List the files in the working directory in long format   
```bash
$ls -l
-rw--------------  1me       me        34653          Sep 21 2023         README.md

-----------------  -------  --------- --------------  -----------------  -----------
File permissions   Owner    Group     Size(in bytes)  Modification Time  File Name
```


>ls -l /etc /bin   
List the files in the /bin directory and the /etc directory in long format

>ls -la ..   
List all files ( even ones with names beginning with a period character, which are normally  hidden ) in the parent of the working directory in long format   

```
$ ls
<file 1> <file 2> <file 3> <folder 1> <folder 2> <folder 3>
```

change directory
```
$ ls
<file 1> <file 2> <file 3> <folder 1> <folder 2> <folder 3>
```

- cd

change directory
```
$ ls
<file 1> <file 2> <file 3> <folder 1> <folder 2> <folder 3>
```


  
