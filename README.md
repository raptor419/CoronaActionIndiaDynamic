# [Django Dashboard Adminator](https://appseed.us/admin-dashboards/django-dashboard-adminator)

**Open-Source Admin Dashboard** coded in **[Django Framework](https://www.djangoproject.com/)** on top of **Adminator Dashboard** design (free version) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).

<br />

## Dashboard Features

- UI-Ready app, SQLite Database, Django Native ORM
- Modular design, clean code-base
- Session-Based Authentication, Forms validation
- Deployment scripts: Heroku, Docker, Gunicorn / Nginx
- UI Kit: **[Adminator Dashboard](https://colorlib.com/polygon/adminator/index.html?ref=appseed)** (Free version) provided by **ColorLib**
- **MIT License**
- Support: Free support via **Github** and (Paid) **24/7 LIVE Support** via [Discord](https://discord.gg/fZC6hup)

<br />

## Deployment Scripts

- **Heroku** - Cloud Application Platform
- **Docker** - execute the app using a sandboxed container
- **Gunicorn** / Nginx - a common used configuration for Django Apps
- **Waitress** - Gunicorn equivalent for Windows.       

<br />

## Dashboard Links

- [Django Dashboard Adminator](https://appseed.us/admin-dashboards/django-dashboard-adminator) - Product page 
- [Django Dashboard Adminator](https://django-dashboard-adminator.appseed.us/login/) - LIVE Demo
- [Django Dashboard Adminator](https://docs.appseed.us/admin-dashboards/django-dashboard-adminator/) - Docs

<br />

## Want more? Go PRO!

PRO versions include **Premium UI Kits**, Lifetime updates and **24/7 LIVE Support** (via [Discord](https://discord.gg/fZC6hup)) 

| [Premium Django Dashboards](https://appseed.us/bundles/django-admin-dashboards-pro) | [Django Dashboard Black PRO](https://appseed.us/admin-dashboards/django-dashboard-black-pro) | [Django Dashboard Dashkit PRO](https://appseed.us/admin-dashboards/django-dashboard-dashkit-pro) |
| --- | --- | --- |
| [![Premium Django Dashboards - Provided by AppSeed.](https://raw.githubusercontent.com/app-generator/static/master/products/django-dashboard-material-pro-screen.png)](https://appseed.us/bundles/django-admin-dashboards-pro)  | [![Django Dashboard Black PRO](https://raw.githubusercontent.com/app-generator/static/master/products/django-dashboard-black-pro-screen.png)](https://appseed.us/admin-dashboards/django-dashboard-black-pro) | [![Django Dashboard Dashkit PRO](https://raw.githubusercontent.com/app-generator/static/master/products/django-dashboard-dashkit-pro-screen.png)](https://appseed.us/admin-dashboards/django-dashboard-dashkit-pro)

<br />
<br />

![Django Dashboard Adminator - Open-Source Web App.](https://raw.githubusercontent.com/app-generator/static/master/products/django-dashboard-adminator-screen.png)

<br />

## How to use it

```bash
$ # Get the code
$ git clone https://github.com/app-generator/django-dashboard-adminator.git
$ cd django-dashboard-adminator
$
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv --no-site-packages env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv --no-site-packages env
$ # .\env\Scripts\activate
$ 
$ # Install modules
$ # SQLIte version
$ pip3 install -r requirements.txt
$
$ # Create tables
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
$
$ # Start the app - custom port 
$ # python manage.py runserver 0.0.0.0:<your_port>
$
$ # Access the web app in browser: http://127.0.0.1:8000/
```

<br />

## Deployment

The app is provided with a basic configuration to be executed in [Heroku](https://heroku.com/), [Docker](https://www.docker.com/), [Gunicorn](https://gunicorn.org/), and [Waitress](https://docs.pylonsproject.org/projects/waitress/en/stable/).

### [Heroku](https://heroku.com/) platform

```bash
$ # Get the code
$ git clone https://github.com/app-generator/django-dashboard-adminator.git
$ cd django-dashboard-adminator
$
$ # Heroku Login
$ heroku login
$
$ # Create the app in Heroku platform
$ heroku create # a random name will be generated by Heroku
$
$ # Disable collect static 
$ heroku config:set DISABLE_COLLECTSTATIC=1
$
$ # Push the source code and trigger the deploy
$ git push heroku master
$
$ # Execute DBSchema Migration
$ heroku run python manage.py makemigrations
$ heroku run python manage.py migrate
$
$ # Visit the deployed app in browser.
$ heroku open
$
$ # Create a superuser
$ heroku run python manage.py createsuperuser
```

<br />

### [Docker](https://www.docker.com/) execution
---

The application can be easily executed in a docker container. The steps:

> Get the code

```bash
$ git clone https://github.com/app-generator/django-dashboard-adminator.git
$ cd django-dashboard-adminator
```

> Start the app in Docker

```bash
$ sudo docker-compose pull && sudo docker-compose build && sudo docker-compose up -d
```

Visit `http://localhost:5005` in your browser. The app should be up & running. 

<br />

### [Gunicorn](https://gunicorn.org/)
---

Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX.

> Install using pip

```bash
$ pip install gunicorn
```
> Start the app using gunicorn binary

```bash
$ gunicorn --bind=0.0.0.0:8001 core.wsgi:application
Serving on http://localhost:8001
```

Visit `http://localhost:8001` in your browser. The app should be up & running.


<br />

### [Waitress](https://docs.pylonsproject.org/projects/waitress/en/stable/)
---

Waitress (Gunicorn equivalent for Windows) is meant to be a production-quality pure-Python WSGI server with very acceptable performance. It has no dependencies except ones that live in the Python standard library.

> Install using pip

```bash
$ pip install waitress
```
> Start the app using [waitress-serve](https://docs.pylonsproject.org/projects/waitress/en/stable/runner.html)

```bash
$ waitress-serve --port=8001 core.wsgi:application
Serving on http://localhost:8001
```

Visit `http://localhost:8001` in your browser. The app should be up & running.

<br />

## Credits & Links

### [Django Admin Dashboards](https://appseed.us/admin-dashboards/django)

Index with UI-ready **admin dashboards** generated by the AppSeed platform in [Django Framework](https://www.djangoproject.com/).
Start fast your next Django project by using functional admin dashboards enhanced with Database, ORM, authentication flow, helpers and deployment scripts.

### What is [Django](https://www.djangoproject.com/)

[Django](https://www.djangoproject.com/) is a Python-based free and open-source web framework, which follows the model-template-view architectural pattern. It is maintained by the Django Software Foundation, an independent organization established as a 501 non-profit. Django's primary goal is to ease the creation of complex, database-driven websites.

### [What is a dashboard](https://en.wikipedia.org/wiki/Dashboard_(business))

A dashboard is a set of pages that are easy to read and offer information to the user in real-time regarding his business. A dashboard usually consists of graphical representations of the current status and trends within an organization. Having a well-designed dashboard will give you the possibility to act and make informed decisions based on the data that your business provides - *definition provided by [Creative-Tim - Free Dashboard Templates](https://www.creative-tim.com/blog/web-design/free-dashboard-templates/?ref=appseed)*.

### [Adminator Dashboard](https://colorlib.com/polygon/adminator/index.html?ref=appseed)

Adminator is a responsive Bootstrap 4 Admin Template. It provides you with a collection of ready to use code snippets and utilities, custom pages, a collection of applications and some useful widgets. Adminator is licensed under The MIT License (MIT) - provided by **ColorLib**.

<br />

---
[Django Dashboard Adminator](https://appseed.us/admin-dashboards/django-dashboard-adminator) - Provided by **AppSeed** [Web App Generator](https://appseed.us/app-generator).
"# CoronaActionIndiaDynamic" 
