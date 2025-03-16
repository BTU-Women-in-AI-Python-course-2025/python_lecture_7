# Django

- **Essence of Web Frameworks**:
  - An introduction to what web frameworks are and why they are used in web development.

- **Overview of the Django Framework**:
  - Discussing the features and components of the Django framework.

- **Installing Django** - https://docs.djangoproject.com/en/5.0/topics/install/:
  - Step-by-step guide on how to install Django on your system.

- **Creating a Simple Django Project** - https://docs.djangoproject.com/en/5.0/intro/tutorial01/:
  - Instructions on setting up a basic Django project and creating a simple application within it.

- **Media and static folders** - https://testdriven.io/blog/django-static-files/

# Django Commands

### `django-admin startproject [project name]`
Creates a new Django project with the specified name. It sets up the basic directory structure and necessary files to start building a Django application.

### `python manage.py migrate`
Applies database migrations, synchronizing the database state with the current set of models and migrations. It creates the necessary database tables and applies any changes to the schema.

### `python manage.py showmigrations`
Lists all migrations available in your Django project and shows whether each one has been applied to the database.

### `python manage.py collectstatic`
Collects all static files from your Django apps and places them in the directory specified by the `STATIC_ROOT` setting. It is typically used when deploying the project to a production server.

### `python manage.py runserver`
Starts the Django development server on the local machine. It allows you to test your application by running it locally and accessing it via a web browser.
