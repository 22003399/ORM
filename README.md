# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2023-06-07 094129](https://github.com/22003399/ORM/assets/121918391/68895c63-3a7f-4d55-b690-18f009139363)
## DESIGN STEPS

### STEP 1:

   Clone the repository from github

### STEP 2:
   Create an admin page for Django.

### STEP 3:
   create an app and edit settings.py

### STEP 4:
   Makemigration and migrate the changes.

### STEP 5:
   Create admin user and write python code for admin and models

### STEP 6:
   Make all the migration to my app

### STEP 7:
   Create a students database with 10 fields using runservercommand
admin.py

from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)

models.py

from django.db import models
from django.contrib import admin

class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')

## OUTPUT
![Screenshot 2023-06-07 094023](https://github.com/22003399/ORM/assets/121918391/40385c17-b8d9-4f34-9a0f-dc6855e32acd)
## RESULT
The program for creating a studentdatabase using ORM is executed successfully.
