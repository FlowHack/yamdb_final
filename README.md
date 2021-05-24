# yamdb_final

Сайт: _http://84.252.140.69/_

![example workflow](https://github.com/FlowHack/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg)

### Описание
_Благодаря этому ресурсу каждый сможет найти информацию по произведениям различных направлений и жанров, а также оставить отзыв или комментарий_

### Технологии
- Python 3.8
- Django 3.0.5

### Запуск проекта
- Установите [Docker](https://docs.docker.com/engine/install/) на свой компьютер
- Запустите контейнер: 
```
docker run flowhack/yamdb
```
- Узнайте ID своего контейнера
```
docker ps
```
- Войдите в bash своего контейнера 
```
docker exec -it <container_id> bash
```
- Выполните команды
```
python3 manage.py makemigrations User
python3 manage.py makemigrations api_reviews
python3 manage.py makemigrations
python3 manage.py migrate
```
- Создайте супер пользователя (следуйте инструкциям)
```
python3 manage.py createsuperuser
```
- Заполните БД стартовыми данными
```
python3 manage.py loaddata fixtures.json
```
- Выйдите из bash командой Ctrl + C

# Готово!