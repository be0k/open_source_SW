# Lab 4
## Linux CLI ( Command Line Interface )
[![Linux](https://softwarelab.org/wp-content/uploads/Linux.jpg)](https://linuxcommand.org)
### Shell command

- `>`

a command to create and save output in a file
```
$ li > file_list.txt
$ cat file_list.txt
a.py
b.ipynb
c.cpp
d.c
e.json
f.pt
```

---
- `cat`

display the content of a text file
```
$ cat file_list.txt
a.py
b.ipynb
c.cpp
d.c
e.json
f.pt
```

---
- `>>`

If it already exists, append output to an extising file.   
not exists, create and write to a new file.
```
$ls >> file_list.txt
$cat file_list.txt
a.py
b.ipynb
x.c
y.cpp
z.pt
```

---
- `<`

redirect input from a file.
can mix `<` and `>` together in a single line.
```
$ cat words.txt
a
c
b
d
$ sort < words.txt > sorted_words.txt
$ cat sorted_words.txt
a
b
c
d
```

---
- `|`

output of previous command to input of next command.
```
$ ls
a
c
d
$ mkdir b | ls
a
b
c
d
```

---
- `echo`

special characters expand its meaning when given to shell commands.
```
$ echo print out the txt
print out the txt

$ echo *
(print filename in current directory)
README.md file_list.txt

$ ehco ~
/home/beok
```

---
- `\`

can be used to ignore line change in command to enter a long cmmand in multiple lines
```
$ ls \
> --reverse \
> --human-readable
total Nk
------ 1 beok beok FILESIZE DATE FILENAME
------ 1 beok beok FILESIZE DATE FILENAME
- rwx  rwx  rwx 1 beok beok FILESIZE DATE FILENAME
- ---  ---  ---
|  |    |    |___ Read, Write, and Excute permissions for all other users
|  |    |________ Read, Write, and Execute permissions for the group woner of the file
|  |_____________ Read, Write, and Execute permissions for the file owner.
|________________ File type('-' indicates regular file, 'd' indicates directory)
```

---
- `chmod`

change permissions   
```
$ chmod 612 some_file
```
6 = 110 = rw- for owner   
1 = 001 = --e for group   
2 = 010 = -w- for others   

---
- `sudo`

If some commands need superuser's privilleges, put "sudo" before the command
```
$ sudo some_command
Password for me:
$
```
```
$sudo -i
Password for me:
root@linuxbox:~#
```

---
- `history`

see previous command history or save it to a text file.
```
# history > history_command.txt
$ cat history
```

---
In Linux, you can choose CLI-based or GUI-based text editors

|**Name**|**Description**|**Interface**|
|---|---|---|
|vi & vim|The granddaddy of Unix text editors, vi, is infamous for its obtuse user interface. On the bright side, vi is powerful, lightweight, and fast. Learning vi is a Unix rite of passage, since it is universally available on Unix-like systems. On most Linux distributions, an enhanced version of vi called vim is provided in place of vi. vim is a remarkable editor and well worth taking the time to learn it.|command line|
|Emacs|The true giant in the world of text editors is Emacs originally written by Richard Stallman, Emacs contains(or can be made to contain) every feature ever conceived of for a text editor. It should be noted that vi and Emacs fans fight bitter religious wars over which is better.|command line|
|nano|nano is a free clone of the text editor supplied with the pine email program. nano is very easy to use but is very short on features compared to vim and emacs. nano is recommended for first-time users who need a command line editor.|command line|
|gedit|gedit is the editor supplied with the GNOME desktop environment. gedit is easy to use and contains enough features to be a good beginners-level editor.|graphical|
|kwrite|kwrite is the "advanced editor" supplied with KDE. It has syntax highlighting, a helpful feature for programmers and script writers.|graphical|
