# Ex02 Django ORM Web Application
## Date: 07.9.23

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
Admin.py

from django.contrib import admin
from .models import Player,PlayerAdmin
admin.site.register(Player,PlayerAdmin)

Models.py

from django.db import models
from django.contrib import admin
class Player (models.Model):
    pid=models.CharField(max_length=20,help_text="Player ID")
    name=models.CharField(max_length=100)
    height=models.IntegerField()
    weight=models.IntegerField()
    phone_no=models.IntegerField()

class PlayerAdmin(admin.ModelAdmin):
    list_display=('pid','name','height','weight','phone_no')
```

## OUTPUT
![Screenshot (37)](https://github.com/LINGARAJA-L/ORM/assets/129825857/ec693984-3eb4-4fe1-8764-73ef5a0b73b9)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
