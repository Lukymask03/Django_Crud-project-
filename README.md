# Django_Crud-project-

# Task Manager
Before running or starting your project, ensure you have the following installed:

- Python (latest Version)
- pip (Python package manager)
- Virtual environment
- Django (install via `pipenv install django` if not already installed)
- mysqlclient (install via `pip install mysqlclient` for MySQL database integration)


### 1. Install (Pip and Virtual Env)
```
pipenv install django
pipenv shell
pip install mysqlclient
```

### 2. Setting Up Django Project
create a new Django project and a new app within that project. run the following commands on your terminal:

```
django-admin startproject project_name
cd project_name
python manage.py startapp app_name
```

### 3. Register App and Database

Include App in the INSTALLED_APPS list:

```
INSTALLED_APPS = [
    'myapp',
]
```

Mysql Database

```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql', <!--Specifies that MySQL is the database backend-->
        'NAME': 'db_name', #Name of the database
        'USER': 'root', #Database username
        'PASSWORD': '', #Database password
        'HOST': 'localhost', #Database host
        'PORT': '3306', #Default MySQL port
    }
}
```

### 4. Defining Models
after setting up/creating the models

Run the following commands to create the migrations:

```
python manage.py makemigrations
python manage.py migrate
```

### 5. Set Up (Templates, URLs Routing, Forms, Views,...etc)

after Setting up, Navigate to project directory (if nasa loob na ng project dir you can skip this.)
```
cd project_name
```

### 6. Start the Development Server

```
python manage.py runserver
```

Click the link and open it to your browser

```
http://127.0.0.1:8000/
```

Append the App's Url path to access a specific app within your project

```
http://127.0.0.1:8000/create/
```

Project set up complete! you can now test your project.
