# How to start Git

## Basic Git
vcs? 
형상관리시스템 (version control system)의 약자이며 소스코드 관리 및 파일 관리를 하는 시스템을 말함
scm?
소스코드관리 (source code management)의 약자이며 말그대로 소스코드 업데이트나 제작 내용을 관리하는 것을 의미

### 단위
- Blob : 대용량 Binary 객체(Binary Large Object)의 약자이며 작업된 공간 전체를 의미
- Tree : Blob의 모음
- commit : Blob 안에서 수정된 log

### Bush 명령어
git status : 현재 git 의 정보를 출력
git log : 수정된 commit의 정보와 현재 작성중인 git의 정보를 출력

## Git configuration
git config : commit 작성에 포함된 정보를 선언
--global [정보 명칭] ["정보 내용"]

```shell
$ git config --global user.name "Developer-Mang"
$ git config --global user.email "chiwon618@gmail.com"
$ git config --global core.editor "vim"
$ git config --global core.pager "cat"
```

## Start to 'git init'
git init : commit 단위 시작을 선언
    Local repository를 생성
git remote add [주소 명칭] [repo 주소] : github 연결할 주소를 지정
git remote get-url [주소 명칭] : 연결된 주소를 출력

## Start to 'git clone'
git clone [repo 주소] : 해당 repo를 복사해서 불러옴

## Upload 'github'
업로드 과정
[WorkSpace]>(add)>[Stage]>(commit)>[local repository]>(push)>[github 서버]

git add [작업된 파일명] : 해당 파일의 작업된 내용을 스테이지에 보냄
git commit : 해당 commit의 shilling을 함
    입력하면 commit의 간단한 설명을 기입한다. 기본으로 vim이 실행
    ! (-m "commit 내용을 기입") : 터미널에서 직접 입력할 수 있다.
git push [repo 주소 명칭] master : local repo에 있는 commit을 해당 github repo에 업로드함

