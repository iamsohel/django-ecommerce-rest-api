# Ecommerce Application
## Description

A boilerplate for starting a django framework based comprehensive e-commerce application 

## Requirements

Software

- [Python 3.11](https://docs.python.org/3/whatsnew/3.11.html)
- MySQL
- Docker

Style Guide

- [Flake8](https://flake8.pycqa.org/en/latest/)

## Features
* Category Management
* Product Management
* Order Management
* Customer Management
* Promotion Management
* Shopping Cart
* Review
* Authentication (jwt login, registration)
* Logging (configured logger to log error)
* Error handling 
* Test case 

## Tech

* Django
* Django Rest Framework
* Flake8
* Swagger
* MySQL
* Docker
* Github Action

### Installation & Run without docker 

follow the below steps

- make virtual environment
    `python -m venv env`
- activate the virtual environment in windows
    `.\env\Scripts\activate`
- activate the virtual environment in linux/mac
    `sourc env_name/bin/activate`
- install the dependency from requirements.txt
    `pip install requirements.txt`

### Installation & Run with docker 

follow the below steps

- run docker compose to up and running the application 
    `docker-compose up`

### Making migrations for a new app (in steps):
- First make and run migrations  without docker
- `python manage.py makemigrations`
- `python manage.py migrate`

- make and run migrations  in docker
- `docker-compose exec web python manage.py makemigrations`
- `docker-compose exec web python manage.py migrate`

### Run test
- Run test without docker
- `python manage.py test`

- run test in docker
- `docker-compose exec django_appetizer_dev_api python manage.py test`
