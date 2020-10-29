# DjangoRestApi
Database used here is MongoDB.
Created an Admin Panel to manage the Users and their details.

Prerequisite:
  1.Create a virtual environmnet:
    >>pip3 install virtualenv
    >>python -m venv my_venv
    Now as you have created virtual environment, named "my_venv", you need to activate it:
    >>my_venv\Scripts\activate.bat
    
   2.Install Django:
    Now in same virtual environment, install django:
    >>pip install django
    
   3.Install Django Rest Framework:
    >>pip install djangorestframework
   
   4.djongo: Djongo is a SQL to mongodb query transpiler. It translates a SQL query string into a mongoDB query document. As a result, all Django features, models etc work as is.
    >>pip install djongo
    
   5.Move to our directory using cd or if you are already in it ignore this.
   
   And follow below instructions for model migration and accessing the panel: 

To get access to this panel:
  1. Connect project to mongoDb database i.e. migrate data model:
        >>python manage.py makemigrations users
        >>python manage.py migrate users
  2. Create a superuser:
        >>python manage.py createsuperuser
     Add your credentials to become superuser.
  3. Runserver:
        >>python manage.py runserver
  4.Get admin panel at:
        127.0.0.1:8000/admin
    You need to add your credential, asked here to get access.
