# How to start Git

## Basic Git
vcs? version control system. System to management about all Binary like scm etc
scm? source code management.

### Unit
- Blob : Binary Large Object. All content like media, source code, .exe etc.
- Tree : group of Blob
- commit : log about modify something in blob

### Bush command
git status : print about git status
git log : print about git and commit information

## Git configuration
git config : Define commit information
--global [info.name] ["content"]

```shell
$ git config --global user.name "Developer-Mang"
$ git config --global user.email "chiwon618@gmail.com"
$ git config --global core.editor "vim"
$ git config --global core.pager "cat"
```

## Start to 'git init'
git init : Define start to commit
    create Local repository
git remote add [repo.name] [repo.url] : Define github address
git remote get-url [repo.name] : print about [repo.name] url

## Start to 'git clone'
git clone [repo address] : Copy repo

## Upload 'github'
Process Upload
[WorkSpace]>(add)>[Stage]>(commit)>[local repository]>(push)>[github 서버]

git add [file.name] : send file(modefied) commit to stage 
git commit : shilling commit
    insert sample commit infomation
    ! (-m "content") : Insert directly into teminal
git push [repo.name] master : send commit to github server

