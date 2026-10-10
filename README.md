# Repository: django-dealership-app

## Project: Best Cars Dealership — Django Application Development with SQL and Databases

A full-stack car dealership web application built with **Django** (backend), **React** (frontend),
**Express.js** (dealer microservice) and **SQLite/PostgreSQL** (database), containerized with Docker
and deployed on IBM Cloud Code Engine with a GitHub Actions CI/CD pipeline.

### Features
- Dealer management backed by an Express.js REST API (`/fetchDealers`, `/fetchDealer/:id`,
  `/fetchDealers/:state`, `/fetchReviews/dealer/:id`)
- Car makes and models managed through Django models (`CarMake`, `CarModel`) and the Django Admin site
- User authentication: login, logout and registration (Django + React)
- Dealer reviews with IBM Watson Natural Language Understanding sentiment analysis
- Static "About Us" and "Contact Us" pages
- CI/CD with GitHub Actions: lint, test, build Docker image, deploy to Code Engine

### Tech stack
Django 4.2 · React 18 · Express.js · SQLite · Docker · IBM Cloud Code Engine · GitHub Actions

### Run locally
```bash
pip install -r requirements.txt
python3 manage.py migrate
python3 manage.py runserver
```
