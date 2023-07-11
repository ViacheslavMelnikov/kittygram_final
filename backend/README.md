### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram_backend.git
```

```
cd kittygram_backend
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

* Если у вас Linux/macOS

    ```
    source env/bin/activate
    ```

* Если у вас windows

    ```
    source env/scripts/activate
    ```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

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

Создать файл переменных окружения .env в корневой директории проекта. 
Пример заполнения файла .env:
```
POSTGRES_DB=kitty
POSTGRES_USER=user
POSTGRES_PASSWORD=passw
DB_NAME=dbsql
DB_HOST=base
DB_PORT=5432
```
Файл .env следует указать в .gitignore для исключения попадания в репозиторий!