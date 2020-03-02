# python instruction

### key command
- MAC - python3 | pip3
- WINDOWS - python | pip

### check version
#### Windows
- python --version
- pip --version
#### Mac
- python3 --version
- pip3 --version


### check setup (Windows)
 pip freeze : check all packages

1. pip install virtualenv
	- install virtual envirnment

2. python -m venv venv
    - -m : make
    - venv : virtual environment
		- run & name

3. run virtual envirnment
	- MAC - source venv/bin/activate
	- WINDOW - . ./venv/Scripts/activate
	- deactivate : ends virtual environment
	
5. pip freeze
	- check to see what is installed on virtual env.

4. pip install Django
	- install Django framework
	- within virtual environment
	- type: "Django" > enter

5. python -m pip install --upgrade pip
	- optional

### use Django

- app folder vs project folder


### create app
- django-admin startproject [app-name]
	- project name & folder name will be the same
- cd [folder-name]
- python ./manage.py startapp [folder-name]
- [folder-name]/settings.py
	- edit 'INSTALLED_APPS' : 
	- add 'client' to bottom

```python
INSTALLED_APPS=[..., 'client']
```

### setup file
- [folder-name]/urls.py
	- set it to home in client

``` python
from django.contrib import admin
from django.urls import path, include

urlpatterns = [

	path("", include('client.urls') )
]
```
- 'include' tell Django to look for certain file 'client.urls'

- create urls.py in file
	- `app/client/urls.py` 
- create file called views

---

### 
. : currentt file to import
