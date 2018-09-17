# Installation


1) Make sure you have at least python 3.5 by typing `$ python --version` on the command line.

***Note for cloud 9 users only***  
You can upgrade your python by typing:
```sh
$ pyenv install 3.5.0    (this will take a while)
$ pyenv global 3.5.0
```

2) Download django

```sh
$ sudo pip install django
```

3) Start a django website

```sh
$ django-admin startproject <project-name>
$ cd <project-name>
```
A django project is divided in one or more apps, that way you can re-use any app on other proyects.

4) Create your first app

```sh
$ python manage.py startapp <app1_name>
```

5) Run the migrations

```sh
$ python manage.py migrate
```

6) Add your website URL to the ALLOWED_HOSTS on settings.py

```python
ALLOWED_HOSTS = [
    '*',
    ]
```


7) Run django on c9 ports by doing 

```sh
$ python manage.py runserver $IP:$PORT
```

## Now start adding endpoints to your API using the following workflow: [Typical workflow for any API method](quick_tutorials/FIRST_APP.md).




### Aditional Tutorials
- [Working with django /admin](quick_tutorials/ADMIN.md) to create superusers, add models to your admin, etc.
- [Using the shell](quick_tutorials/DATABASE_API.md) to CRUD models, etc.
- [Working with Migrations](quick_tutorials/MIGRATIONS.md) for everytime you change your model
- [Using MySQL](quick_tutorials/MYSQL.md) insalling and using MySQL in your application.
- [Using Mongo](quick_tutorials/MONGO.md) insalling and using mongo in your application.
- [Working with OAuth](quick_tutorials/OAUTH.md) implementing OAuth with the JWT Oauth Toolkit.
