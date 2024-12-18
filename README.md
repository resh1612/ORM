# Ex02 Django ORM Web Application
# Date: 4.12.2024
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
```
 admin.py

 from django.contrib import admin 

 from.models import Loan,LoanAdmin

 admin.site.register(Loan,LoanAdmin)
 
 models.py

 from django.db import models

 from django.contrib import admin
 
 class Loan(models.Model):
 
 Name=models.CharField(max_length=10)
 
 Accountno=models.IntegerField(primary_key="Refno")
 
 Address=models.CharField(max_length=30)
 
 Aadharno=models.IntegerField()
 
 Email=models.EmailField()
 
 class LoanAdmin(admin.ModelAdmin):
 
 list_display=('Name','Accountno','Address','Aadharno','Email')
```

# OUTPUT

![WhatsApp Image 2024-12-18 at 12 40 39_ba275942](https://github.com/user-attachments/assets/ae517b66-0ee7-4576-a834-35a537e5445c)
![WhatsApp Image 2024-12-18 at 12 41 11_b828230e](https://github.com/user-attachments/assets/f84edc4e-9117-4bde-a937-dd57b79cca4e)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
