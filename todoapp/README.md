Простой Тобо менеджер, реализованный на веб-фреймворке Django В качестве веб-интерфейса использован фреймворк Semantic UI https://semantic-vi.com/

Создаем папку для нового проекта и переходим в нее

md ToDoDjango & cd TaDoDjango


Устанавливаем и активируем виртуальное окружение

pythons -m venv venv

• venv/bin/activate


Инициализируем git

git init


Устанавливаем модули

pip install django gunicorn


Создаем проект todoapp и переходим в него

django-admin startproject todoapp & cd todoapp

Создадим приложение todolist

python manage.py startapp todolist

Зарегистрируем приложение в файле settings.py

 INSTALLED_APPS = [
****
todolist,
 ]

Укажем локализацию и часовой пояс в файле settings-py

LANGUAGE_CODE = 'ru'
TIME_ZONE = 'Asia/Bishkek'
TEMPLATES = 'DIRS: ['templates']

Создадим моделидля приложения. класс ToDo и доп.класс Meta

Производим миграцию

python manage.py makemigrations

python manage.py migrate

создаем суперпользователя командой:

python manage.py createsuperuser

Запускаем приложение и проверяем работоспособность в админке

python manage.py runserver

