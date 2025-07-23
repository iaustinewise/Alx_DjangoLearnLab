# Exploration of Project Structure

- **manage.py**: A command-line utility located at the root of the outer LibraryProject directory, used to interact with this Django project. It runs the development server (e.g., `python manage.py runserver`), applies migrations (e.g., `python manage.py migrate`), creates superusers, and manages the project.
- **settings.py**: Configuration file located in the inner LibraryProject directory, defining settings like `DEBUG` (True for development), `INSTALLED_APPS` (includes admin, auth, contenttypes, sessions, messages, and staticfiles), `DATABASES` (uses SQLite3 with db.sqlite3), and `TIME_ZONE` (set to UTC).
- **urls.py**: The URL declarations file in the inner LibraryProject directory, acting as a “table of contents” by mapping URLs (e.g., admin) to views, currently including the default welcome page at the root URL.
