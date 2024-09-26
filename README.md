# QickHub service for registration and user profile


### Описание

---------

Привет, это тестовый сервис, который тебе нужно дописать вместе с твоим напарником. Это сервис для брони аудиторий в корпусах

### Необходимые улучшения для Frontend

---
* Реализовать верстку согласно [макету] (http://ссылка)
* Различные анимации реализовать с помощью JavaScript
* Стили прописывать с помощью CSS

### Необходимые улучшения для Backend

---
* Реализовать базовый функционал (прописано в TODO)
* Подключить loguru
* Изменить модель Reservation и всё, что с ней связано таким образом, что бы только зарегистрированные пользователи могли бронировать аудитории. Реализовать систему регистрации
* Реализовать систему кэширования внутри приложения

### Инструкция по запуску на локальной машине в debug режиме

----

Для того, что-бы запустить приложение на локальной машине в debug режиме нужно выполнить следующие шаги:


0) Дописать базовй функционал проекта со стороны Backend (или отключить недописанные части шаблона)
1) Запустите контейнер командой:
2) Собрать Docker контейнер через файл **docker-compose.yml**. Выполните команду:
    ```commandline
    docker-compose build
    ```
3) Запустите контейнер командой:
    ```commandline
    docker-compose up
    ```
4) Применить миграции к проекту если вы запустили данную версию сервиса впервые. Это можно сделать следующей командой, введенной в новом окне командной строки:
    ```commandline
    docker-compose run --rm web-app sh -c "python manage.py migrate"
    ```

### Инструкция по запуску unit tests

---

Для запуска unit тестов необходимо:
1) запустить проект как описано выше
2) прописать следующую команду
   ```commandline
   docker-compose run --rm web-app sh -c "python manage.py test"
   ```
   
---
### Дополнительное
---

Пока вы работаете над этим сервисом можете писать вашему тимлиду по любым вопросам в любое время :) 
   
---

### Если у вас есть идеи по улучшению этого сервиса или предложения по добавлению нового функционала, пожалуйста, добавляйте их сюда.

---