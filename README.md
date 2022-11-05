### Описание:

API для социальной сети блогеров Yatube.

### Использованные технологии:

Django==2.2.16

pytest==6.2.4

pytest-pythonpath==0.7.3

pytest-django==4.4.0

djangorestframework==3.12.4

djangorestframework-simplejwt==4.7.2

Pillow==8.3.1

PyJWT==2.1.0

requests==2.26.0

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/IvanCh-dev/api_final_yatube.git
```

```
cd yatube_api
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

### Примеры некоторых запросов к API:

Получение всех публикаций:

```
GET /api/v1/posts/
```

Создание публикации:

```
POST /api/v1/posts/

Payload
{
  "text": "string",
  "image": "string",
  "group": 0
}
```

Получение публикации:

```
GET /api/v1/posts/{id}/
```

Получение всех комментариев к публикации:

```
GET /api/v1/posts/{post_id}/comments/
```

### Об авторе:

IvanCh-dev
