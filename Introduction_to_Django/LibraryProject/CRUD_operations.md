# CRUD Operations for Book Model


## Individual Markdown Files

### create.md
```markdown
# Create Operation

**Command:**
```python
from bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)

**Expected Output:**
```python
# A Book instance is created with id=1, no output is displayed in the shell

### retrieve.md
```markdown
# Retrieve Operation

**Command:**
```python
from bookshelf.models import Book
book = Book.objects.get(title="1984")
print(book.title, book.author, book.publication_year)

**Expected Output:**
```python
# 1984 George Orwell 1949


### update.md
```markdown
# Update Operation

**Command:**
```python
from bookshelf.models import Book
book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()
print(book.title)

**Expected Output:**
```python
# Nineteen Eighty-four


### delete.md
```markdown
# Delete Operation

**Command:**
```python
from bookshelf.models import Book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()
print(Book.objects.all())

**Expected Output:**
```python
# <QuerySet []> 

