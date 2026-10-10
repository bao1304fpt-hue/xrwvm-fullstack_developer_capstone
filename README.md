# Repository: xrwvm-fullstack_developer_capstone

## Project: fullstack_developer_capstone

A full-stack car dealership web application built with **Django** (backend), **React** (frontend),
**Express.js** (dealer microservice) and **SQLite/PostgreSQL** (database), containerized with Docker
and deployed with a GitHub Actions CI/CD pipeline.

### Features
- Dealer management backed by an Express.js REST API (`/fetchDealers`, `/fetchDealer/:id`,
  `/fetchDealers/:state`, `/fetchReviews/dealer/:id`)
- Car makes and models managed through Django models (`CarMake`, `CarModel`) and the Django Admin site
- User authentication: login, logout and registration (Django + React)
- Dealer reviews with IBM Watson Natural Language Understanding sentiment analysis
- Static "About Us" and "Contact Us" pages
- CI/CD with GitHub Actions: lint Python files, lint JavaScript files, test, build Docker image, deploy

### Tech stack
Django 4.2 · React 18 · Express.js · SQLite · Docker · GitHub Actions

### Run locally
```bash
pip install -r requirements.txt
python3 manage.py migrate
python3 manage.py runserver
```
