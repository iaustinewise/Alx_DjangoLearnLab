# Create Operation
```python
from bookshelf.models import Book
book = Book(title="1984", author="George Orwell", publication_year=1949)
book.save()
- Expected Output: No error, book created successfully.
