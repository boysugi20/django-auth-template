# Django Allauth Custom User Template

## Description

The Django Allauth Custom User Template is a starting template for Django projects that provides pre-configured authentication using Django Allauth and a custom user model. It helps developers quickly set up a Django project with user registration, login, and logout functionalities, utilizing the powerful features of Django Allauth while incorporating a custom user model to suit specific project requirements. This template serves as a solid foundation for building web applications with user authentication capabilities in Django.

## Table of Contents

- [Setup](#setup)
- [Requirements](#requirements)
- [Configurations](#configurations)

## Setup

Follow these steps to set up the project locally:

1. Install project dependencies using Pipenv:<br />
`pipenv install`
2. Reset the database:<br />
`python manage.py reset_db`
3. Apply database migrations:<br />
`python manage.py migrate`
4. Start the development server:<br />
`python manage.py runserver`
4. Start the tailwind server:<br />
`python manage.py tailwind start`

## Requirements

Ensure the following prerequisites are met before running the project:

- **Node.js and npm:**: Install npm to manage and compile Tailwind CSS styles.
- **Windows Users**: Uncomment the "NPM_BIN_PATH" in the settings.py file.

## Configurations

Follow these steps to change the project name:

1. Rename the Project Directory:<br />
`mv myProject newProjectName`
2. Update `manage.py` and `myProject/wsgi.py`:<br />
change:
`os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'myProject.settings')`
into:
`os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'newProjectName.settings')`
3. Update `myProject/settings.py`:<br />
change:
`ROOT_URLCONF = 'myProject.urls'` and `WSGI_APPLICATION = 'myProject.wsgi.application`
into:
`ROOT_URLCONF = 'newProjectName.urls'` and `WSGI_APPLICATION = 'newProjectName.wsgi.application`