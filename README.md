
# Ex02 Django ORM Web Application
# Date: 28-09-2025
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

admin.py
from django.contrib import admin

from.models import Car,CarAdmin

admin.site.register(Car,CarAdmin)

#Resgister your models here.

models.py
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
    price = models.CharField()m
    description = models.TextField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_brand', 'car_model', 'year', 'color', 'engine_type', 'fuel_type', 'transmission', 'seating_capacity', 'price', 'description')
# OUTPUT
.<img width="1920" height="1080" alt="Screenshot 2025-09-28 001542" src="https://github.com/user-attachments/assets/78191d10-da1e-40e0-9599-ed26e7b1db1a" />


# RESULT
Thus the program for creating a database using ORM has been executed successfully
