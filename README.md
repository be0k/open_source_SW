# temp-repo
### This repository will be ref_Git.
### If you didn't know info that you want,      please `git help <commend-name>` or go https://git-scm.com/docs
### Three areas
1. Working directory
2. Stating area
3. Repository

### First step -> ` git init `

#### If you use git first,
```
git config user.name 'YOUR-NAME'
git config user.email 'YOUR-EMAIL'
```
## Simple Using git
### Initial Setting(No README.md)
```
echo "CONTENT" >> README.md
git add . (OR) git add README.md
git commit -m "EXPLANATION"
git branch -M main
git remote add origin "REPOSITORY-LINK"
git push -u origin main
```

### Initial Setting(Existing README.md)
```
git remote add origin "REPOSITORY-LINK"
git branch -M main
git push -u origin main
```

### When you push again
```
git pull
git add .
git commit -m "EXPLANATION"
git push (origin main)
```


## Useful code
### Delete .git in working directory
`rm -rf .git`

### Forcing push
`git push -f origin "BRANCH-NAME"`

###  


## Explaining frequently used code
* `git init` : 현재 디렉토리를 git이 관리하는 working directory로 설정하고 그 안에 repository 생성

* `git add`
  > git add <file-name> : 수정사항이 있는 특정 파일을 staging area에 올리기
  > git add <directory-name> : 해당 directory 내에서 수정사항이 있는 모든 파일들을 staging area에 올리기
  > git add . : working directory 내에 있는 수정사항이 있는 모든 파일들을 staging area에 올리기

* `git reset`
  > git reset <file-name> : staging area에 올렸던 파일 다시 내리기(git status를 통해 확인)
  > git reset <option> <commit-id> : option에 따라 작업이 달라짐(deefalut option == --mixed)
  > > 1. HEAD가 특정 commit을 가리키도록 이동시킴(--soft)
  > > 2. staging area도 특정 commit처럼 리셋(--mixed)
  > > 3. working directory도 특정 commit처럼 리셋(--hard)
  > > commit-id 대신 (HEAD^, HEAD~n)같은 표기법을 통해 위치 기준으로 설정 가능
* `git status` : git이 현재 인식하고 있는 프로젝트 관련 내용들을 출력
* `git commit`
  > git commit : 이 코드만 사용하면 메세지를 쓸 수 있는 vim 창이 열림(나오는 방법 -> esc 누르고 :wq입력 후 enter)
  > git commit -m "MESSEGE" : 현재 staging area에 있는 것들 commit으로 남기기
  > git commit --amend : 최신 커밋을 다시 수정해서 새로운 commit으로 만듬(messege 수정)
* `git log`
* `git log --pretty=oneline`
* `git show`
* `git commit --amend`
* `git config alias.`
* `git diff`
* `git tag`
* `git pull`
* `git push`
* `git clone`
* `git branch`
* `git checkout -b`
* `git switch`
* `git branch -d`
* `git merge`
* `git merge --abort`
* `git fetch`
* `git blame`
* `git revert`
* `git reflog`
* `git log --all --graph`
* `git rebase`
* `git stash`
* `git cherry-pick`
