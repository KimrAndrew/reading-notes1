# [Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)

Django ships with a built-in User model
Django docs highly reccomend using a custom model

## Setup

- create and navigate into the `accounts` directory
- install Django
- make a new Django project called `config`
- start the local web server

```BASH
$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ poetry add django
$ poetry shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver
```

- `migrate` has purposefully not been run

## AbstratctUser vs AbstractBaseUser

Two modern wayst to create a custom user model:
- `AbstractUser`
- `AbstractBaseUser`

`AbstractBaseUser` requires more work so we'll be using `AbstractUser` which subclasses `AbstractBaseUser`

## Custom User Model

Creating the model takes four steps:

- update `config/settings.py`
- create a new `CustomUser` model
- create new `UserCreation` and `UserChangeForm`
- update the admin

Add `accounts` app to `INSTALLED_APPS` in `settings.py`
Set `AUTH_USER_MODEL` to our new custom model

```python
# config/settings.py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'accounts', # new
]
...
AUTH_USER_MODEL = 'accounts.CustomUser' # new
```

Update `admin.py` with our new User Model

```python
# accounts/admin.py
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin

from .forms import CustomUserCreationForm, CustomUserChangeForm
from .models import CustomUser

class CustomUserAdmin(UserAdmin):
    add_form = CustomUserCreationForm
    form = CustomUserChangeForm
    model = CustomUser
    list_display = ['email', 'username',]

admin.site.register(CustomUser, CustomUserAdmin)
```

Run `makemigrations` and `migrate` to create a new database with the custom user model
