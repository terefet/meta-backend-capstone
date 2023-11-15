# meta-backend-capstone
python -m venv venv
source .venv/bin/activate
pip install django
# create a django project
django-admin startproject littlelemon
# run development server
cd littlelemon
python manage.py runserver
# create a django app 
python manage.py startapp restaurant
# install client
pip3 install mysqlclient

python3 manage.py migrate 
python3 manage.py makemigrations
python manage.py createsuperuser
#user:admin
#email: admin@gmail.com
#password: 1234
pip3 install djangorestframework


pip install djoser

navigate to http://127.0.0.1:8000/auth/token/login/ to get the token

use http://127.0.0.1:8000/auth/token/logout/ to logout with the token in the header

GET in http://localhost:8000/api/menu-items/
GET in http://localhost:8000/api/menu-items/1

GET in http://localhost:8000/api/booking/
GET in http://localhost:8000/api/booking/1
