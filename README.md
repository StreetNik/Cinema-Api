# Cinema Api

***

API service for cinema management writen on DRF

## Installing using GitHub

***

Install PostgreSQL and create database

```Python
git clone https://github.com/StreetNik/Cinema-Api.git
cd Cinema_Api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set POSTGRES_HOST=<your db hostname>
set POSTGRES_NAME=<your db name>
set POSTGRES_USER=<your db user>
set POSTGRES_PASSWORD=<your db user password>
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

## Run with docker

***

Docker should be installed

```
docker-compose build
docker-compose up
```

## Getting access

***

* create user via /api/user/register/
* get access token via /api/user/token/


## Features

***

* JWT authenticated
* Admin panel /admin/
* Documentation is located at /api/doc/swagger/
* Managing order and tickets
* Creating movies with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions