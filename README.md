# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2025-05-16 212356](https://github.com/user-attachments/assets/96374dd8-4db1-489b-ace9-685701f6de52)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)
model.py
from django.db import models
from django.contrib import admin
class Bankloan (models.Model):
    acc=models.IntegerField(primary_key="acc")
    name=models.CharField(max_length=100)
    mobileno=models.IntegerField()
    pancode=models.IntegerField()
    aadharcode=models.IntegerField()
class BankloanAdmin(admin.ModelAdmin):
    list_display=('acc','name','mobileno','pancode','aadharcode')
```
# OUTPUT
![Screenshot 2025-05-16 212420](https://github.com/user-attachments/assets/61e255b2-7b70-413c-9b7d-459b522d6d2c)
![Screenshot 2025-05-16 212506](https://github.com/user-attachments/assets/ea72ff00-a646-447c-82c3-907fac7c874b)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
