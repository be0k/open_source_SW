### First step
```
$ git config --global user.name <YOUR_NAME>
$ git config --global user.email <YOUR_EMAIL>
$ git config --global init.defaultBranch main
$ git config --list
$ git config --list --show-origin
$ git config user.name
<YOUR_NAME> 
```

* `git version` : check pre-installed version
* `git init` : change current directory to working directory that git manages and generate repository in there.
* `git status` :print contents about projects that git is currently cognizing.

* `git add`
  > git add <file-name> : add modified specific file to staging area.   
  > git add <directory-name> : add modified files in that directory to staging area.    
  > git add . : add modified files in working directory to staging area.

* `git rm --cashed <file-name>` : except file from staging area.

* `.gitignore` : files in this file are ignored adding.
  > *.a : ignore all .a files   
  > !lib.a : but do track lib.a, even though you're ignoring .a files above.    
  > /YODO : only ingnore the TODO file in the current directory, not subdir /TODO.    
  > build/ : ignore all files in any directory named build.    
  > doc/*.txt : ignore doc/notes.txt, but not doc/server/arch.txt.     
  > doc/**/*.pdf : ignore all .pdf files in the doc/ directory and any of its subdirectories.

* `git commit`
  > git commit : open vim that can type commit message.   
  > git commit -m "MESSEGE" : commit files currently remaining

* `git log` : print commit history

* `git branch`
  > git branch <new-branch-name> : create new branch   
  > git branch -m <old-name> <new-name> : change old-name to new-name

