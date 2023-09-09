# temp-repo
### This repository will be ref_Git.

### Three area
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


## Explaining code
* `git init`
* `git add`
* `git reset`
* `
