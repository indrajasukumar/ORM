# Ex02 Django ORM Web Application
## Date:11-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
<img width="451" alt="er diagram booklist ss" src="https://github.com/indrajasukumar/ORM/assets/145115195/bafabd55-df34-4a32-b705-a3a40b023ad7">



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

```
models.py
class Book(models.Model):
  Book_id=models.IntegerField(primary_key=True);
  Book_author=models.CharField(max_length=20);
  Book_name=models.CharField(max_length=50);
  publication=models.DateField();
  price=models.IntegerField();
class BookAdmin(admin.ModelAdmin):
  list_display=("Book_id","Book_author","Book_name","publication","price");

admin.py
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
```


## OUTPUT
<img width="958" alt="booklist ss" src="https://github.com/indrajasukumar/ORM/assets/145115195/64c9d224-4460-4004-b078-445a5f9d3d94">




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
