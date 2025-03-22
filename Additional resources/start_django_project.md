# Django Installation and Project Setup Guide

This guide will walk you through the steps to install Django and create a new Django project from scratch.

---

## Table of Contents
1. [Install Python](#1-install-python)
2. [Install Django](#2-install-django)
3. [Create a New Django Project](#3-create-a-new-django-project)
4. [Run the Development Server](#4-run-the-development-server)
5. [Run Migrations](#5-run-migrations)
6. [Create a Superuser](#6-create-a-superuser)
7. [Access the Admin Panel](#7-access-the-admin-panel)

---

## 1. Install Python

Before installing Django, ensure you have Python installed. Django requires Python 3.8 or higher.

### Check Python Version
Run the following command to check your Python version:
```bash
python --version
```
or
```bash
python3 --version
```

### Install Python (if not installed)
- **Windows**: Download and install Python from [python.org](https://www.python.org/downloads/).
- **macOS**: Use Homebrew to install Python:
  ```bash
  brew install python
  ```
- **Linux**: Use your package manager:
  ```bash
  sudo apt update
  sudo apt install python3
  ```

---

## 2. Install Django

Once Python is installed, you can install Django using `pip`, the Python package manager.

### Install Django
```bash
pip install django
```

### Verify Installation
Check the Django version to confirm the installation:
```bash
django-admin --version
```

---

## 3. Create a New Django Project

To start a new Django project, use the `django-admin` command.

### Create Project
```bash
django-admin startproject projectname
```
Replace `projectname` with the name of your project. This will create a directory with the following structure:
```
projectname/
├── manage.py
└── projectname/
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    ├── asgi.py
    └── wsgi.py
```

---

## 4. Run the Development Server

Navigate into your project directory and start the development server.

### Navigate to Project Directory
```bash
cd projectname
```

### Run the Server
```bash
python manage.py runserver
```

### Access the Project
Open your browser and go to `http://127.0.0.1:8000/`. You should see the Django welcome page.

---

## 5. Run Migrations

Migrations are used to apply changes to your database schema.

### Create Migrations
```bash
python manage.py makemigrations
```

### Apply Migrations
```bash
python manage.py migrate
```

---

## 6. Create a Superuser

To access the Django admin panel, create a superuser (admin account).

### Create Superuser
```bash
python manage.py createsuperuser
```
Follow the prompts to enter a username, email, and password.

---

## 7. Access the Admin Panel

Once the superuser is created, you can access the Django admin panel.

### Start the Server
```bash
python manage.py runserver
```

### Access Admin Panel
Go to `http://127.0.0.1:8000/admin/` and log in with your superuser credentials.

---
