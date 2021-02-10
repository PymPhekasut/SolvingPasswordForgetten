# SolvingPasswordForgetten
How to solve basic problem when user forget password to log in on Django


1. Open CMD
2. Go to folder where locate Django project
3. Type: python manage.py shell



```
>>> from django.contrib.auth.models import User
>>> User.objects.all()
<QuerySet [<User: All users>]>
>>> admin = User.objects.get(username='User_name')
>>> User_name
<User: User_name>
>>> type(User_name)
<class 'django.contrib.auth.models.User'>
>>> admin.set_password('1234')
>>> admin.save()
```
