## Git 연결

git bash 실행
git config --global user.name "DanielKim-D"
git config --global user.email "protoco@naver.com"
git config --list

## 원격 레포지토리를 확인

git remote -v

## 끊고자 할때

git remote remove {레파지토리 이름}

## 새 레포지토리에 연결하고 싶을때

git remote add {레파지토리 이름} "깃허브 주소"

## 이후 원하는 동작 ex) push

git push -u {레파지토리 이름} push

## 연결 계정 변경하는 법

git config -- global user.name "계정 이름"
git config -- global user.email "계정 이메일 주소 "

## 로컬에서 생성한 브랜치 원격에 올리기

올리고 싶은 브랜치로 이동한 뒤
git push

## 브랜치 생성

git branch -M {branch name}

## 브랜치 이동

git switch {branch name}

## 브랜치 생성

그 후 기능 구현을 위해 브랜치를 생성하자.(기본은 main으로 되어있음)
git checkout -b [branch name]