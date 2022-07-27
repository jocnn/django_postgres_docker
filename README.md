Web Django con Postgres y Docker
===
Abstract: Applicación Django Web ejecutado en Docker y Postgres, se configuro 2 servicios uno para web Django y otro para DB Postgres, la primera con dependencia al servicio db 
## Information
- Title:  `Django Web`
- Authors:  `jocnn`

## Install & Dependence
- asgiref==3.5.2
- black==22.6.0
- click==8.1.3
- Django==4.0.6
- mypy-extensions==0.4.3
- pathspec==0.9.0
- platformdirs==2.5.2
- sqlparse==0.4.2
- tomli==2.0.1
- psycopg2-binary==2.9.3

## Use
- for docker
```
  > docker-compose up -d --build
  > docker-compose exec web python manage.py migrate
  > docker-compose exec web python manage.py createsuperuser
  > docker-compose down
```

## Directory Hierarchy
```
|—— .dockerignore
|—— .gitignore
|—— .venv
|—— Dockerfile
|—— db.sqlite3
|—— django_project
|    |—— __init__.py
|    |—— __pycache__
|        |—— __init__.cpython-310.pyc
|        |—— settings.cpython-310.pyc
|        |—— urls.cpython-310.pyc
|        |—— wsgi.cpython-310.pyc
|    |—— asgi.py
|    |—— settings.py
|    |—— urls.py
|    |—— wsgi.py
|—— docker-compose.yaml
|—— manage.py
|—— requirements.txt
```
