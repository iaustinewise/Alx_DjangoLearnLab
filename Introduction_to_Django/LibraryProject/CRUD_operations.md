# CRUD Operations Documentation

This document outlines the basic CRUD (Create, Read, Update, Delete) operations performed on the `Book` model in the `bookshelf` app.

## Create
```python
from bookshelf.models import Book
book = Book(title="1984", author="George Orwell", publication_year=1949)
book.save()

- Expected Output: No error, book created successfully.

## Read
```python
book = Book.objects.get(title="1984")
print(book.title, book.author, book.publication_year)

- Expected Output: 1984 George Orwell 1949


## Update
'''python
book.title = "Nineteen Eighty-Four"
book.save()
print(book.title, book.author, book.publication_year)

- Expected Output: Nineteen Eighty-Four George Orwell 1949
Delete

## Delete
'''python
book.delete()
Book.objects.all()

- Expected Output: (1, {'bookshelf.Book': 1}) followed by <QuerySet []>

