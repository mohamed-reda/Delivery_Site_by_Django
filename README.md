## Delivery Site by Django


safely collect and handle data while maintaining a user-friendly experience 

It has:
- creating users and data 
- access stored data with SQLite
- creating a dynamic template
- deploy forms to your site
- leverage submitted form data
- work with widgets, customize formsets


<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_1.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_2.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_4.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_5.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_6.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_7.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_8.png?raw=true" width="800" height="400"  />  

<img src="https://github.com/mohamed-reda/Delivery_Site_by_Django/blob/master/screansots/img_9.png?raw=true" width="800" height="400"  />  





## commands

1 

pipenv install django~=3.1.14 

pip install django

~= which will ensure security updates for Django, such as 3.1.1, 3.1.2, and so on.

------------------------------------------------------------------------------

check

django-admin --version

------------------------------------------------------------------------------

activate virtual environment:

pipenv shell

------------------------------------------------------------------------------

if this runs with no error:

2

django-admin startproject nandiasgarden .

so my virtual environment has Django installed properly.

here without (.) to the command, it will create config folder in config folder

------------------------------------------------------------------------------

3

django-admin startapp pizza


4

pip3 install django-widget-tweaks 



------------------------------------------------------------------------------

running Django’s local web server

python manage.py runserver

exit

------------------------------------------------------------------------------

pipenv shell

exit


------------------------------------------------------------------------------

python manage.py startapp pages

• admin.py is a configuration file for the built-in Django Admin app

• apps.py is a configuration file for the app itself

• migrations/ keeps track of any changes to our models.py file so our database and models.py stay in sync

• models.py is where we define our database models which Django automatically translates into database tables

• tests.py is for our app-specific tests

• views.py is where we handle the request/response logic for our web app

------------------------------------------------------------------------------
Run:

python manage.py runserver

------------------------------------------------------------------------------
test:

python manage.py test

------------------------------------------------------------------------------

apply the migrations:

python manage.py migrate

change the user:

python manage.py createsuperuser

nilecrocodile

mohamed.reda.007007@gmail.com 

12345678

------------------------------------------------------------------------------
after creating new model at notes, lets deal with the database:

python manage.py makemigrations

after showing the migration of which user who created the note, apply the default athe terminal as:

1

1

then apply the migrations:

python manage.py migrate

check:

python manage.py shell

from django.contrib.auth.models import User

user = User.objects.get(pk=1)

user

user.notes.count()

------------------------------------------------------------------------------
