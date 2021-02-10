# student-management-system2

## This is a simple API for: 
* creating a unified interface for keeping track of freeCodeSchool students 
* accounts for students to login and see their own pages 
* admins can login and see everyone via the Django admin interface 
* it will be able to use Github OAuth

## About the Program

* freeCodeSchool is a non-profit coding program that teaches people coding basics for free.
* It's set up to offer 3-month long classes in two different levels, 1 and 2.
  When students pass level 1 - HTML, CSS, and JS, they can move onto level 2 - Node, Express, and Mongo.

## Table of Contents

* [Requirements](#requirements)
* [Schema](#schema)
* [API](#api)
* [Roadmap](#roadmap)

## Running Locally

1. Must have Python 3 & Postgres version 12.x installed and running
1. Clone the repo and cd into repo
1. Create a virtual environment: `python -m venv venv`
1. Go into your virtual environment: `source venv/bin/activate`
1. Install dependencies: `pip install -r requirements.txt`
1. Create an admin user for logging into the Django admin interface: `python manage.py createsuperuser`
1. Setup Database
    1. Create the database: `CREATE DATABASE freecodeschool;`
    1. Create DB user: `CREATE USER fcs_admin;
    1. Grant privilages to user for our database: `GRANT ALL PRIVILEGES ON DATABASE freecodeschool TO fcs_admin;`
    1. Run migrations: `python manage.py migrate`
1. Run the app: `python manage.py runserver`
1. View the API at `localhost:8000` and the admin interface at `localhost:8000/admin`



