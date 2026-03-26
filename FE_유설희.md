## Git, Github

Git : 내 컴퓨터에서 버전 관리를 하는 프로그램
Github : Git을 온라인으로 공유할 수 있는 플랫폼

## 주요 Git 명령어 정리

- git init : 이 폴더를 깃허브와 연동 (.git 생성됨)
- git remote add origin 개인레포주소 : 원격 저장소 연결
- git remote -v : 연결된 원격 저장소 확인
- git branch -M main : 기본 브랜치 이름 master->main으로 변경
- git pull origin main : 깃허브의 main branch의 최신 사항 반영
- git add . : 현재 디렉토리 아래의 모든 변경 파일을 git이 추적
- git commit -m "커밋메세지" : 추적한 파일들을 실제 git 이력에 기록
- git push origin main : 커밋한 수정사항들을 origin 레포의 main 브랜치에 올림
- git branch : branch 목록 확인
- git branch 새브랜치이름 : 새 브랜치 생성
- git switch 브랜치 이름 : 브랜치 이동
- git branch -d 브랜치 이름 : 해당 브랜치 삭제

## Git 충돌 해결

- PR에서 충돌 해결하는 경우 (Web Editor)
- pull을 받아 vscode로 해결하는 경우

## Django

- Framework : 소프트웨어 개발을 효율적으로 만들어주는 도구
