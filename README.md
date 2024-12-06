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
admin.py

from django.contrib import admin

from .models import BankLoan

admin.site.register(BankLoan)

models.py

from django.db import models

class BankLoan(models.Model):
    
    loan_id = models.AutoField(primary_key=True)  # Primary Key (Auto Incremented)
    
    customer_name = models.CharField(max_length=255)  # Name of the loan customer
    
    loan_amount = models.DecimalField(max_digits=15, decimal_places=2)  # Total loan amount
    
    loan_term_years = models.PositiveIntegerField()  # Loan term in years
    
    interest_rate = models.DecimalField(max_digits=5, decimal_places=2)  # Interest rate
    
    loan_status = models.CharField(max_length=50, choices=[('Approved', 'Approved'), ('Pending', 'Pending'), ('Rejected', 'Rejected')])  # Loan status

    def __str__(self):
    
        return f"{self.customer_name} - {self.loan_amount}"



# OUTPUT

![WhatsApp Image 2024-12-06 at 22 38 58_95942683](https://github.com/user-attachments/assets/0557f761-5ba8-4ba4-942a-c391afe3f2e8)

![WhatsApp Image 2024-12-06 at 23 05 22_9eeb8341](https://github.com/user-attachments/assets/82f61e87-ee18-4672-bf11-9ce34d0f4d9b)

![WhatsApp Image 2024-12-06 at 23 05 45_dc708e96](https://github.com/user-attachments/assets/cc776cce-7697-4714-9b8a-767a185d31ac)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
