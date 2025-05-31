# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).
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
.. admin.py

from django.contrib import admin from .models import Employee,EmployeeAdmin admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models from django.contrib import admin

class Employee(models.Model): eid = models.CharField(max_length=20,help_text="Employee") name = models.CharField(max_length=100) age = models.IntegerField() salary=models.IntegerField() email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin): list_display=('eid','name','age','salary','email')

...



# OUTPUT
![image](https://github.com/user-attachments/assets/2dc7e0b0-8d54-4f30-b966-18a838a60c13)
![image](https://github.com/user-attachments/assets/6a94c3f5-e930-4363-afea-292828ae0650)
![image](https://github.com/user-attachments/assets/459b78e2-3c23-4f61-b556-ad225ead4f85)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
