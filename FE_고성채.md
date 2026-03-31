 # 14th_git_hw
2026-03-25 내용 요약

1. git 사용법(개인)
    - 프로젝트 처음에 1번만
        1. Github에서 개인 레포지토리 생성
        2. 로컬에서 폴더 생성 후, 사용자 등록
        3. 생성한 개인 레포지토리에 연결
    - 프로젝트 내내 반복
        1. 폴더에서 파일 수정, 편집
        2. 폴더에서 파일 수정 사항 반영 (add,commit)
        3. 폴더를 push하여 개인 레포지토리에 반영

2. git 사용법(협업)
    - 프로젝트 처음에 한번만
        1. Github에서 레포지토리 생성(=중앙레포지토리)
        2. 각 팀원들은 해당 중앙레포지토리를 fork하여 개인 레포지토리 생성
        3. 폴더 생성 후, 중앙레포지토리와 개인레포지토리에 연결 (origin, upstream)
    - 프로젝트 내내 반복
        1. 작업 시작하기 전 upstream에서 !!! PULL !!!
        2. Branch 생성, 폴더에서 파일 수정, 편집
        3. 폴더에서 파일 수정 사항 반영 (add, commit)
        4. 폴더를 push하여 개인 레포지토리에 반영 
        5. 개인 레포지토리에서 Pull Request 하기
        6. 중앙 레포지토리에서 코드 확인 후 Merge 받기
        7. 폴더의 main 브랜치에 수정사항 반영
        8. 예전 브랜치 삭제 (3.5~10반복)

3. 충돌 발생 시
    - Web Editor를 통한 충돌 해결
    - pull을 받아 vscode로 해결
    
    - 결론: pull을 잘 하자 !!

4. Django 세팅
    1. 가상환경 설정하기
        - python -m venv venv: 'venv'라는 이름의 가상환경 생성
        - source venv/Scripts/activate: 가상환경 활성화 (Windows 기준)

    2. gittgnore 생성
        - touch .gitignore: gitignore 파일 생성

    3. gitignore 설정
        - https://www.toptal.com/developers/gitignore/ 에 들어가서
        - macOS , Windows , VisualStudioCode, venv, Django 검색 후 붙여넣기

    4. Django 설치 및 프로젝트 생성
        - pip install django: 장고 라이브러리 설치
        - django-admin startproject [프로젝트명] . : 현재 폴더에 프로젝트 생성 (뒤에 . 필수)

    5. settings.py 설정
        - ALLOWED_HOSTS = ['*']        --- 접근 가능한 호스트 설정 ( '*' : 모든 사용자 접근 가능 )
        - LANGUAGE_CODE = 'ko-kr'      --- 언어 설정을 대한민국으로
        - TIME_ZONE = 'Asia/Seoul'     --- 시간 설정을 대한민국으로
        - USE_I18N = True              --- Djandgo내 다국어 지원 가능
        - USE_TZ = False               --- 로컬 시간 사용하지 않음

    6. APP 생성
        - python manage.py startapp [app name]: 앱 설치(app name은 main으로)(manage.py 파일이 있는 디렉토리에서 startapp 명령어를 입력)
        - settings.py에 INSTALLED_APPS에 main(설치한 앱) 등록

    7. 서버 실행
        - python manage.py makemigrations: 모델 변경 사항 감지
        - python manage.py migrate: 변경 사항을 데이터베이스에 반영
        - python manage.py runserver: 개발 서버 실행

    8. git에 연동
        - git add .
        - git commit -m "커밋메시지"
        - git branch -M main
        - git remote add origin [개인레포 주소]
        - git remote -v
        - git push origin main