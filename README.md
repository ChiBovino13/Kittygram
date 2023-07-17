# Проект «Kittygram»
____
**Описание:**
Django-проект Kittygram: управление котиками. Позволяет пользователям регистрироваться и добавлять на сайт фотографии котиков.
____
## Технологии:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)  \
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)  \
![DjangoREST](https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=gray)  \
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)  \
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
### 🎉🐚  Как запустить проект  ⛵♣

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram.git
```

```
cd kittygram
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```



# Примеры работы с 𝔸ℙ𝕀 для всех пользователей:
Публикция, редактирование и удаление контента доступно только авторизированным пользователям.
Неавторизированные пользователи могут работать с API только в режиме чтения.

```
GET api/v1/cats/ - страница котиков;
GET api/v1/cats/{id}/ - страница конкретного котика по его id;
GET api/v1/owners/ - страница пользователей (хозяев котиков);
GET api/v1/owners/{id}/ - страница конкретного пользователя по его id.
```
## Примеры запросов и ответов

### Создание поста:
```JSON
POST /api/v1/cats/
```
в body

```JSON

{
    "name": "Барсик",
    "color": "White",
    "birth_year": 2011
} 
```
### Обновление поста:
```JSON
PUT /api/v1/cats/{id}/
```
в body

```JSON

{
    "name": "Барсик",
    "color": "White",
    "birth_year": 2021
} 
```
### Удаление поста:
```JSON
DEL /api/v1/cats/{id}/
```

**♘😈  Автор:  ♙🎉** [Дарья Горячева](https://github.com/ChiBovino13)
