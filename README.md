# infra_sprint1
Проект Kittygram
Kittygram — социальная сеть для обмена фотографиями любимых питомцев.

Используемые технологии:
Django 3.2.3
Python 3.10.6
Django REST Framework 3.12.4
Nginx 1.18.0
Gunicorn 20.1.0

Как запустить проект:

Для развёртывания проекта необходимо скачать его в нужную вам директорию, например:
git clone git@github.com:...../infra_sprint1.git

В директории infra_sprint1/backend/ создайте файл .env с переменными окружения:
SECRET_KEY='your secret key'
ALLOWED_HOSTS=список разрешенных хостов

Cоздать и активировать виртуальное окружение:
python3 -m venv env
source env/bin/activate

Установить зависимости из файла requirements.txt:
python3 -m pip install --upgrade pip
pip install -r requirements.txt

Выполнить миграции:
python3 manage.py migrate

Назначьте текущего пользователя владельцем директории media 
sudo chown -R <имя_пользователя> /var/www/kittygram/media/

Запустить проект
