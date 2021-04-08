Microtask 4:
Set up the developer environment of SortingHat (muggle branch).

1. Clone the repository, and change to the muggle branch

```
$ git clone https://github.com/chaoss/grimoirelab-sortinghat
$ git checkout muggle
```

2. Installed the poetry

3. Installed the libmysqlclient-dev

4. Installed the required dependencies
```
$ poetry install
```

5. Activate the virtual environment:
```
$ poetry shell
```

6. Migrations, fixtures and created a superuser:
```
(.venv)$ ./manage.py makemigrations --settings=config.settings.devel
(.venv)$ ./manage.py migrate --settings=config.settings.devel
(.venv)$ ./manage.py loaddata sortinghat/core/fixtures/countries.json --settings=config.settings.devel
(.venv)$ ./manage.py createsuperuser --settings=config.settings.devel
```

7. Run SortingHat backend Django app:
```
(.venv)$ ./manage.py runserver --settings=config.settings.devel
```

8. Installed npm

9. Installed yarn
```
npm install -g yarn
```

10. Installed the required dependencies
```
$ cd ui/
$ yarn install
```

11. Run SortingHat frontend Vue app:
```
$ yarn serve
```

