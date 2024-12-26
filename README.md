# Ex02 Django ORM Web Application
# Date:20/09/24
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM:
![Screenshot 2024-12-07 100938](https://github.com/user-attachments/assets/87310812-0189-46ed-bea9-f9801e96c305)

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

~~~
admin.py:
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

models.py:
from django.db import models
from django.contrib import admin
class Book(models.Model): 
       Author_name=models.CharField(max_length=20,primary_key=True)
       Co_Author_name=models.CharField(max_length=20)
       Book_Name=models.CharField(max_length=50)
       Edition=models.CharField(max_length=20)
       Year=models.IntegerField()
       Publisher=models.CharField(max_length=50)

class BookAdmin(admin.ModelAdmin):
       list_display=('Author_name','Co_Author_name','Book_Name','Edition','Year','Publisher')

~~~
# OUTPUT
![alt text](<Screenshot 2024-12-04 141914.png>)
![alt text](<Screenshot 2024-12-05 201657.png>)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
