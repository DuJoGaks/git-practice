# [OSS] Git-1 Week6_Lab6  
#### 202234880 Kimtaewoo  
---
### Git config : First time setup  
- git config --global
- user.name / user.email / init.defaultBranch main
- git init to initializing a repo
```sh
$ git config --global 
$ git config --list --show-origin
$ git init
```

### git three stage
- Modified -> Staged -> commited
1. make file in working directory
2. stage fixes to staging area
3. commit to git directory(repository)

---

## Shell Things - Git  
### Git status  
- git status
- to check current repository's status
```sh
$ git status
```
### Git add  
- git add [file name]
- to adding new file to be "staged"
- git add . to staging current directory's all file
```sh
$ git add Readme.md
$ git add .
$ git status
```
### Git remove staged file
- git rm
- to remove file by "staged"
```sh
$ git rm --cached [file_name]
$ git status
```
## Git commit
- git commit -m "message"
- to commit staged file
```sh
$ git commit -m "init commit"
```
---
## Etc.
- edit .gitignore to set ignoring files
- git branch -m [name] [new name] to rename branch