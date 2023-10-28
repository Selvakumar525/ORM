# Ex02 Django ORM Web Application
## Date: 27/10/2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

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
~~~
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

Models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    age=models.CharField(max_length=100)
    email=models.CharField(max_length=100)

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','age','email')
~~~

## OUTPUT

![image](https://github.com/Selvakumar525/ORM/assets/120643262/17df760f-9fd0-49f7-a1c6-002205377615)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
