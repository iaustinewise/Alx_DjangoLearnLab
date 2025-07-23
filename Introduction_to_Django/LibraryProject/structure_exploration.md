# Exploration of Project Structure

- **manage.py**: A command-line utility that lets you interact with this Django project. It is used to run the development server (e.g., `python manage.py runserver`), apply migrations, and manage the project.
- **settings.py**: Configuration file for the Django project, defining settings like `DEBUG`, `INSTALLED_APPS` (e.g., admin, auth), `DATABASES` (using SQLite), and `TIME_ZONE` (set to UTC).
- **urls.py**: The URL declarations for the project, acting as a “table of contents” by mapping URLs (e.g., admin) to views, currently including the default welcome page.
