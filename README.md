1. git 사용법(개인)
git init                        # 저장소 초기화
git add .                       # 전체 스테이징
git commit -m "메시지"           # 커밋
git log --oneline               # 커밋 기록 확인
git status                      # 현재 상태 확인

2. git 사용법(협업)
git clone [URL]                 # 원격 저장소 복제
git remote add origin [URL]     # 원격 저장소 연결
git push origin main            # 원격에 올리기
git pull origin main            # 원격에서 가져오기
git branch BE_HJH               # 브랜치 생성
git checkout BE_HJH             # 브랜치 이동
git merge BE_HJH                # 브랜치 병합

3. git 충돌

4. Django 개발환경 세팅
python -m venv venv             # 가상환경 생성
source venv/Scripts/activate    # 가상환경 활성화 (Windows)
pip install django              # Django 설치
django-admin startproject 프로젝트명  # 프로젝트 생성
python manage.py startapp 앱명  # 앱 생성
python manage.py runserver      # 서버 실행