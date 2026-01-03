# Ex01 Django ORM Web Application
## Date: 25.11.2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
models.py
```
from django.db import models
from django.contrib import admin
class car(models.Model):
    registerID=models.CharField(max_length=20,help_text="register ID")
    name=models.CharField(max_length=100)
    price=models.IntegerField()
    year=models.IntegerField()

class carAdmin(admin.ModelAdmin):
    list_display=('registerID','name','price','year')

```
admin.py
```
from django.contrib import admin
from .models import car,carAdmin
admin.site.register(car,carAdmin)

```



## OUTPUT

![alt text](<Screenshot 2025-11-24 1418281.png>)

## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
