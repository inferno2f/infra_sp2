# API YAMDB
API для получения информации и обсуждения наиболее интересных произведений

## Стэк технологий:
- Python
- Django Rest Framework
- Postgres
- Docker
### Документация и возможности API:
К проекту подключен redoc. Для просмотра документации используйте эндпойнт `redoc/`

### Квикстарт:

- Склонируйте репозитрий на свой компьютер
- Из папки `infra/` соберите образ при помощи docker-compsoe
`$ docker-compose up -d --build`
- Примените миграции
`$ docker-compose exec web python manage.py migrate`
- Соберите статику
`$ docker-compose exec web python manage.py collectstatic --no-input`
- Для доступа к админке не забудьте создать суперюзера
`$ docker-compose exec web python manage.py createsuperuser`
