# Django Allauth Custom User Template

## Description

The Django Allauth Custom User Template is a starting template for Django projects that provides pre-configured authentication using Django Allauth and a custom user model. It helps developers quickly set up a Django project with user registration, login, and logout functionalities, utilizing the powerful features of Django Allauth while incorporating a custom user model to suit specific project requirements. This template serves as a solid foundation for building web applications with user authentication capabilities in Django.

## Table of Contents

- [Setup](#setup)
- [Configuration](#configuration)

## Setup

Follow these steps to set up the project locally:

1. Create a `.env` file in the root directory with the following content:<br /><br />
DB_NAME=<br />
DB_USERNAME=<br />
DB_PASS=<br />
DB_HOST=<br />
DB_PORT=<br /><br />
Fill in the values for your database configuration.

2. Install project dependencies using Pipenv:<br />
`pipenv install`
3. Reset the database:<br />
`python manage.py reset_db`
4. Apply database migrations:<br />
`python manage.py migrate`
5. Start the development server:<br />
`python manage.py runserver`

## Configuration

Make sure to update the `.env` file with your actual database configuration. Fill in the values for the following variables:

- `DB_NAME`: The name of the database.
- `DB_USERNAME`: The username for database access.
- `DB_PASS`: The password for database access.
- `DB_HOST`: The host or IP address of the database server.
- `DB_PORT`: The port number for database access.
