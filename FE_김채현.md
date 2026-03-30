깃과 깃허브에 대해 알아보고 사용법을 익혔다.
레포지토리를 생성하고 fork, pull request 하는 방법까지 알 수 있었다.
Django 세팅도 했다!

# 개념
git : 분산 버전 관리 시스템
github : git을 온라인으로 공유할 수 있는 플랫폼
Django : 소프트웨어 개발을 효율적으로 만들어주는 도구

# 핵심 코드
git init : 폴더를 깃허브와 연동
git remote add origin 레포지토리 주소 : 원격 저장소 연결
git remote -v : 연결된 원격 저장소 확인
git branch -M main : 기본 브랜치 이름 master→main으로 변경
git pull origin main : 깃허브의 main branch의 최신 사항 반영
git add . : 변경 파일 git이 추적
git commit -m “커밋 메세지" : 실제 Git 이력에 커밋 메세지 기록
git push origin main : 커밋한 정보를 main 브랜치에 올리기