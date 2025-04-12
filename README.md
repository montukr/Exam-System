# Exam System

## Overview
This project is developed using Django, a high-level Python web framework, along with additional dependencies to enhance its functionality. Follow the steps below to set up the environment and run the application on your local machine.

## Prerequisites
- **Python**: Ensure Python is installed on your system. You can download it from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/).
- **pip**: Python's package manager should also be installed. Verify installation by running:
  
  ```bash
  python3 --version
  pip3 --version
  ```

## Installation Instructions

### Step 1: Setting Up the Environment
1. Create a virtual environment (recommended):
   
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

### Step 2: Install Dependencies
Install all the required dependencies listed in the `requirements.txt` file:
   
   ```bash
   pip install -r requirements.txt
   ```

Alternatively, you can install the packages manually:

   ```bash
   pip install asgiref==3.2.7
   pip install Django==3.0.5
   pip install django-widget-tweaks==1.4.8
   pip install pytz==2020.1
   pip install sqlparse==0.3.1
   pip install Pillow
   ```

### Step 3: Setting Up the Database
Run the following commands to set up the database:

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

### Step 4: Create an Admin Account
Create a superuser account to access the admin panel:

   ```bash
   python manage.py createsuperuser
   ```

### Step 5: Run the Application
Start the development server:

   ```bash
   python manage.py runserver
   ```

You can now access the application in your browser at `http://127.0.0.1:8000/`.

## Additional Notes
- **For Admin Account**: Create one using the `createsuperuser` command to manage the application.
- Use the following commands as a reference for setting up the project:

  ```bash
  python3 --version
  pip3 --version
  pip install django
  python3 -m venv venv
  source venv/bin/activate
  pip install Pillow
  python manage.py makemigrations
  python manage.py migrate
  python manage.py createsuperuser
  python manage.py runserver
  ```

## Requirements
The project depends on the following Python packages:
- asgiref==3.2.7
- Django==3.0.5
- django-widget-tweaks==1.4.8
- pytz==2020.1
- sqlparse==0.3.1
- Pillow

These packages are listed in the `requirements.txt` file for easy installation.

---

**Happy Coding!**