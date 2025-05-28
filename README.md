## О проекте

Kittygram - это приложение для обмена фотографиями котиков. Оно позволяет пользователям загружать, просматривать фотографии котиков.

## Технологии

При работе над проектом были применены следующие технологии:
    - PostgreSQL
    - Docker и Docker-Compose
    - JavaScript


### Установка для Windows:

Клонировать репозиторий:

```
git clone https://github.com/chudyashovFAN/kittygram_final
```

Запустить контейнеры

```
docker compose up
```

Выгрузить статику и выполнить миграции:

```
docker compose exec backend python manage.py collectstatic
docker compose exec backend cp -r /app/collected_static/. /backend_static/static/
```

```
python3 manage.py migrate
```
