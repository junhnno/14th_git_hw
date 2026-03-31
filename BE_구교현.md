# 멋쟁이사자처럼 14기 Git & Django 

##  1. Git 

### 초기 세팅 (최초 1회) 

git config --global user.name "깃허브아이디"   
git config --global user.email "깃허브이메일"  

### 기본 사용법 
git init   
git remote add origin 내레포주소   
git remote add upstream 중앙레포주소  
git branch -M main   
git pull origin main     
git branch 브랜치이름   
git switch 브랜치이름 

git add .   
git commit -m "커밋 메세지"   
git push origin main   

## 2. Django  

### 가상환경
python -m venv venv   
source venv/Scripts/activate   

### Django 설치 생성
pip install django   
django-admin startproject project .  
python manage.py startapp main   

### 개발환경 세팅
INSTALLED_APPS = [   
    # ... 기존 코드 ...      
    'main', # 앱 등록    
]  

LANGUAGE_CODE = 'ko-kr'  
TIME_ZONE = 'Asia/Seoul'  
USE_I18N = True  
USE_TZ = False  

### 서버 실행
python manage.py migrate   
python manage.py makemigrations   
python manage.py runserver 