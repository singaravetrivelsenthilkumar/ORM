# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Entity Relationship Diagram](./DOM1.png)

## DESIGN STEPS

### STEP 1:
Apply all the migrations to the myapp


### STEP 2:
Run django admin


### STEP 3:
Create users in the Employee link under'myapp'


## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
## OUTPUT
![OUTPUT](./Tom.png)

## RESULT
The program is executed successfully