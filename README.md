# Ex02 Django ORM Web Application
## Date: 23.04.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-12-19 140514](https://github.com/user-attachments/assets/fcc4838f-9c95-4352-8ee0-938547400357)


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
admin.py
from django.contrib import admin
from .models import Movies,MoviesAdmin
admin.site.register(Movies,MoviesAdmin)


models.py

from django.db import models
from django.contrib import admin
class Movies(models.Model):
    userid=models.IntegerField(primary_key=True)
    username=models.CharField(max_length=30)
    mobileno=models.IntegerField()
    emailid=models.EmailField()
    moviename=models.CharField(max_length=50)
    noofseats=models.IntegerField()
    date=models.DateField()

class MoviesAdmin(admin.ModelAdmin):
    list_display=('username','moviename','noofseats','emailid)
```




## OUTPUT
![web orm](https://github.com/user-attachments/assets/21477ed3-40ec-4337-8ec5-b9c2afbee509)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
