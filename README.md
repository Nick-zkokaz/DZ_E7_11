# ДЗ E7.11

Доска объявлений (с mongodb и кэшем)
 
Сервис на локальном серверe под Windows  и докером c Django:
1) Выполните следующие команды для запуска redis и mongodb:
   
      - docker pull redis:5.0.7
      - docker pull mongo:4.2.3
      - docker run --name redis-instance --rm -d -p 6379:6379 redis:5.0.7 redis-server --appendonly yes
      - docker run --name mongo-instance --rm -d -p "27017:27017" mongo:4.2.3
2) Распакуйте архив с проектом в папку C:/DZ_E7_11
3) В командной строке  директории проекта:
   Выполните команды:
   - python -m venv django
   - C:/DZ_E7_11/django/Scripts/activate.bat 
   - pip install -r requirements.txt
   - python manage.py migrate
   - python manage.py loaddata data.json
   - python manage.py runserver


Проект откроется на http://127.0.0.1:8000.

По умолчанию логин и пароль для пользователя-администратора в проекте:
- Логин: pws_admin
- Пароль: pws_password
