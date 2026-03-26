- GIT: 내 컴퓨터에서 버전 관리를 하는 프로그램
- GITHUB: GIT을 온라인으로 공유할 수 있는 플랫폼

- GIT 사용법 (개인)
1. Github에서 개인 레포지토리 생성
2. 로컬에서 폴더 생성 후 사용자 등록
3. 생성한 개인 레포지토리에 연결

* .gitignore란?
= Git에 올라가면 안되는 파일들을 커밋 대상자에서 제외시키는 파일

* git pull origin main
: 깃허브의 main branch의 최신 사항 반영할게요.

* git push origin main
: 커밋한 수정사항들을 Origin 레포의 mainm 브랜치에 올릴게요.

* git add . 
: 현재 디렉토리(.) 아래의 모든 변경 파일을 git이 추적

- GIT 사용법 (협업)
1. Github에서 레포지토리 생성(=중앙 레포지토리)
2. 각 팀원들은 해당 중앙레포지토리를 fork하여 개인 레포지토리 생성
3. 폴더 생성 후, 중앙 레포지토리와 개인 레포지토리에 연결

* Fork란?
: 다른 사람의 레포지토리를 내 Github 계정으로 복사해오는 것

* Clone이란?
: 다른 사람의 레포지토리를 내 로컬(PC)에 복사해오는 것

* git branch : branch 목록 확인
* git branch 새 브랜치 이름 : 새 브랜치 생성
* git switch 브랜치 이름 : 브랜치 이동
* git branch -d 브랜치 이름 : 해당 브랜치 삭제

* GIT 충돌이란?
: 깃이 스스로 판단하기 어려운 수정사항이 발생했을 때, 사용자에게 해결을 요청하는 상태

- Django 개발환경 세팅
1. 가상환경 설정하기
2. .gitignore 생성
3. settings.py 설정
4. APP 생성
5. 서버 실행
6. git 연동 git에 올리기

- project : 웹사이트 전체를 의미하는 것 

- app : 게시판, 로그인 기능의 집합 단위