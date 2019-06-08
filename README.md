# dynamic-forms

Create dynamic forms application using Django web framework

## Built With

Python - Programming language
Django - Web framework
Django-fobi - Form generator/builder application for Django

## Versions

16/08/2018 prototype

## Installation

Prerequisites
Python >= 3.6.x
pip or pip3
virtualenv
virtualenvwrapper
$ python -V o python3 -V
$ Python 3.6.6
$ pip -V
$ "command not found"
$ pip3 install --upgrade pip
$ pip -V
$ pip 18.0 from /Library/Frameworks/..../pip (python 3.6)
$ pip install --upgrade pip
$ pip install virtualenv virtualenvwrapper

## Getting Started

clone this project

## Creating the develop environment

[user_home]$ mkdir .virtualenv
$ nano .virtualenv
add this
export WORKON_HOME=$HOME/.virtualenvs
change the path to virtualenvwrapper.sh because depends of your system
source /Library/Frameworks/Python.framework/Versions/3.6/bin/virtualenvwrapper.sh (change the path if necessary)
export PIP_VIRTUALENV_BASE=$WORK_HOME 

## Create a virtual environment

$ virtualenv apolloOne
$ source .virtualenv/apolloOne/bin/activate
(apolloOne)$ command...

## Installing

Go to folder that you had cloned the git project.
(apolloOne)$ cd [django_site_root_folder]
(apolloOne)$ pip install -r requirements.txt
(apolloOne)$ python manage.py migrate
(apolloOne)$ python manage.py createsuperuser --username admin
(apolloOne)$ python manage.py runserver [IP:][port number optional ex. 8000 or 127.0.0.1:8000]

## Open your browser and navigate to here

http://localhost:8000
super user administration: admin / apolloadm1n
usuarios agentes:
agente1 / apolloadm1n
agente2 / apolloadm1n

django-admin and manage.py commands
django-admin and manage.py commands (ES)
django-admin and manage.py commands (EN)

## Reset and rebuild

This will IRREVERSIBLY DESTROY all data currently in the database, and return each table to an empty state.
(apolloOne)$ cd [django_site_root_folder]
(apolloOne)$ python manage.py showmigrations
(apolloOne)$ python manage.py flush
(apolloOne)$ python manage.py migrate
(apolloOne)$ python manage.py createsuperuser --name=admin --email=adminnoreal@apollo.apo
(apolloOne)$ python manage.py runserver

## Create a new django application

(apolloOne)$ cd [django_site_root_folder]
(apolloOne)$ python manage.py startapp [application name]
RESULT
app_name/
    migrations/
        __init__.py
    __init__.py
    admin.py
    apps.py
    models.py
    tests.py
    views.py
views.py is the file to create the views for call the view we need to assign the view to a URL to do that we need create a URLConf in urls.py file.
urls.py is the file to create de URLConf.
At last we need to add this urls.py file with the URLConf in the root of the django site in the main file urls.py, the main file urls.py is into the folder that contains settings.py.
If you need more information about django framework works review the django documentation:
Django website
Django website Documentation 2.1 (ES)
Django website Documentation 2.1 (EN)
