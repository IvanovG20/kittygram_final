#  Веб-проект Kittygram
## Описание проекта

Сайт с возможностью публикации котов и кошек, их дней рождений и достижений

## Технологии
- Python 3.9
- Django 3.2.3
- Django REST Framework 3.12.4

## Запуск проекта

1) Клонируйте репозиторий с github
  git clone git@github.com:IvanovG20/kittygram_final.git
2) Запустите проект командой
  sudo docker compose -f docker-compose.yml up

## Сбор статики и применение миграций
После запуска проекта нужно собрать статику и миграции

sudo docker compose -f (file_name_docker-compose.yml) exec backend python manage.py migrate

sudo docker compose -f (file_name_docker-compose.yml) exec backend python manage.py collectstatic

sudo docker compose -f (file_name_docker-compose.yml) exec backend cp -r /app/collected_static/. /static/static/

Проект будет доступен по адресу
http://localhost:9000/

