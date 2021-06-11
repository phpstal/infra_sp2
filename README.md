≡ Краткое руководство LittleSocNet

# Описание проекта LittleSocNet

Данное приложение является очень упрощенной социальной сетью. Пользователи этой сети могут публиковать свои посты, оставлять комментарии и подписываться на интересных им авторов других статей. Вот собственно и все. 
Чем богаты ). 
***

## Запуск на "чистом" Django 
### Команды для запуска приложения

Для запуска проекта на чистом Django нужно в консоли Bash сначала активировать виртуальное окружение, а потом установить все необходимые компоненты в это окружение.
Для этого перейдите в консоли в корень проекта и наберите команду:

**source /venv/script/activate** 

После этого в консоли наберите команду:

**pip install -r requirements.txt**

Затем нужно сделать миграции. Это делается командой:

**python manage.py migrate**

После этого, когда все будет установлено, запустите сервер командой:

**python manage.py runserver**

Всё! Ваш сервер запущен и по адресу http://127.0.0.1:8000 вам будет достна главная страница проекта.
Если хотите сервер остановить, то просто нажмите сочетание клавиш `Ctrl` + `C`
***

### Создание суперпользователя

Данный персонаж все же нужен. Без него трудно будет администрировать ваш проект. Поэтому нужно создать суперпользователя. Это делается командой:

**python manage.py createsuperuser**

Далее указываете имя пользователя, потом пишите его e-mail, два раза пароль. И вуаля, суперюзер создан!
***

### Заполнение базы начальными данными

Для заполнения вашей базы данных можно воспользоваться
тестовой БД на **SqLite**
Скачайте архив по этой [ссылке](https://code.s3.yandex.net/backend-developer/learning-materials/db.sqlite3.zip)
Скачайте файл, извлеките его из архива и замените им ваш файл db.sqlite3. Вместо вашей БД у вас будет база, заполненная тестовыми постами.
