Python-Django based online event platform named stegolica.

Is in opencode.

> Hosting can be done at openshift and webapp is optimised for that.

# Features

1. Question page with hint
2. Ranking page
3. Login and register page

### Try on Heroku
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

Installation
----------  

- `sudo apt-get install libpq-dev python-dev`
- `sudo apt-get install postgresql-server-dev-9.5`

then create an user using 

- `sudo -u postgres createuser -P -s -e <user_name>`

go to wsgi and create a virtualenv

- `cd wsgi`
- `virtualenv venv`
- `source venv/bin/activate`

create a database

- `sudo -u postgres createdb -O <user_name> stegolica`

enable settings, fill in your username and password (of postgres) in settings.py

- `cd stegolica`
- `cp dev-settings.py settings.py`

Do migrations (bare with me)

- `python mange.py migrate`

Run it

- `python manage.py runserver`

go to `127.0.0.1:8000` to view


> for deployment i openshift use dev.py.

Wanna help
---------
you can help by

1. finding out issues
2. fixing issues already in the issues section

Template design
--------------
## main page

![alt text](http://i.imgsafe.org/87195dec93.png)

## login page

![alt text](http://i.imgsafe.org/871922cf5d.png)

## Question page with hint

![alt text](http://i.imgsafe.org/879d151076.png)

Frontend
--------
Uses [materializecss](http://materializecss.com/) and particle.js 

