# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
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
URLs.py

from django.contrib import admin
from django.urls import path

urlpatterns = [
    path('admin/', admin.site.urls),
]

Models.py

from django.db import models
from django.contrib import admin

class Car(models.Model):
    car_brand = models.CharField()
    car_model = models.CharField()
    year = models.DateField()
    color = models.CharField()
    engine_type = models.CharField()
    fuel_type = models.CharField()
    transmission = models.CharField()
    seating_capacity = models.IntegerField()
    price = models.CharField()
    description = models.TextField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_brand', 'car_model', 'year', 'color', 'engine_type', 'fuel_type', 'transmission', 'seating_capacity', 'price', 'description')
    
admin.py

from django.contrib import admin

from.models import Car,CarAdmin

admin.site.register(Car,CarAdmin)

# OUTPUT
<img width="1920" height="1080" alt="Screenshot 2025-09-28 001542" src="https://github.com/user-attachments/assets/15bf8526-8d61-49a2-8dcd-d1e6664db167" />


# RESULT
Thus the program for creating a database using ORM has been executed successfully
