# ToDo application using Django REST Framework. 
It is a basic applicaion in which you can add a task, edit the task, delete the task and filter them according to their status.

# Technology stack
We have used,

1. Python 3
2. Django REST Framework
3. sqlite3 Database

# Project Structure

├── task
│   ├── admin.py
│   ├── apps.py
│   ├── __init__.py
│   ├── migrations: database migrations
│   ├── models.py: database models for task app
│   ├── serializers.py: serializers for the models
│   ├── tests.py: test cases for view
│   ├── urls.py: url endpoints of task app
│   └── views.py: These views are called by API endpoints
├── manage.py
└── todo
    ├── __init__.py
    ├── settings.py: settings file for the project
    ├── urls.py: base urls for apps of the project
    └── wsgi.py
    
# Running Locally
First, clone the repository to your local machine:

git clone https://github.com/saiyadfaizan/REST_todo_.git

cd todo

# Create super user 
python manage.py createsuperuser 

Note: It will prompt to enter username, email and password one by one. Please remember the username and password,
it will be used to login admin area or to hit an API to scrap/refresh the linkedin profiles.

# Steps to run the project

1. Check for the database migrations: python manage.py makemigrations
2. Apply the database migrations: python manage.py migrate
3. Run the developement server: python manage.py runserver
4. Open chrome and the site will be available at 127.0.0.1:8000.
