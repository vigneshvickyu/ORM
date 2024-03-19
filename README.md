# Ex02 Django ORM Web Application
## Date: 19:03:24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

![WhatsApp Image 2024-03-15 at 09 06 47_7d209c3f](https://github.com/selvasachein/ORM/assets/151948835/ad65bdb3-7ec6-4106-949b-963d60457f53)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
models.py

from django.db import models
from django.contrib import admin
class Railway_db(models.Model):
    trainno=models.IntegerField(primary_key=True);
    trainname=models.CharField(max_length=20);
    departure=models.CharField(max_length=50);
    arrival=models.CharField(max_length=50);
    distance=models.IntegerField();
class Railway_dbAdmin(admin.ModelAdmin):
    list_display=("trainno","trainname","departure","arrival","distance");

admin.py

from django.contrib import admin
from .models import Railway_db,Railway_dbAdmin
admin.site.register(Railway_db,Railway_dbAdmin)
```
## OUTPUT

![screen short 2](https://github.com/vigneshvickyu/ORM/assets/151948835/31e452bc-9221-4e99-b424-d714a9e76bc4)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
