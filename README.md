# Ex02 Django ORM Web Application
# Date: 14-12-2024
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
~~~
admin.py

  from django.contrib import admin
  from .models import Bank,BankAdmin
  admin.site.register(Bank,BankAdmin)

models.py

  from django.db import models
  from django.contrib import admin
  
  class Bank(models.Model):
    
      bank_name=models.CharField(max_length=100)
      branch_name=models.CharField(max_length=100)
      customer_name=models.CharField(max_length=100) 
      account_no=models.IntegerField()
      mobile_no=models.IntegerField()
      Email=models.EmailField()
  
  class BankAdmin(admin.ModelAdmin):
      	list_display= ('bank_name', 'branch_name', 'customer_name', 'account_no', 'mobile_no','Email')
~~~
# OUTPUT
![Screenshot (101)](https://github.com/user-attachments/assets/f9709a21-6ed0-4d40-a3ab-693933da42be)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
