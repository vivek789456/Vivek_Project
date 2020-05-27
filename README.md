# Vivek_Project
Fullthrottle Backend Exercise Solution

Execute the command below to start python virtual environment.

virtualenv venv
Execute the command below to execute python virtual environment.

source venv/bin/activate
execute the command below to install modules for the project.

pip install -r requirements.txt
you need to modify mysite/settings.py to connect your database like below.

...
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'django_response_model_to_json',  # DB name
        'USER': 'root',  # DB account
        'PASSWORD': '',  # DB account's password
        'HOST': '127.0.0.1',  # DB address(IP)
        'PORT': '3306',  # DB port(normally 3306)
    }
}
...
execute the command below to migrate.

# python manage.py makemigrations
python manage.py migrate
execute the command below to create django administrator.

python manage.py createsuperuser
execute the command below to insert data. (Data seed)

python manage.py loaddata blog/fixtures/vivek.json
execute the command below to start django test server.

python manage.py runserver
you can see the data stored well on the administrator page.

administrator page: http://127.0.0.1:8000/admin
