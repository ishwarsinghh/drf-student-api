# Student Management API (Django REST Framework)

## Overview
A robust, modular backend REST API built with Django and the Django REST Framework (DRF) to manage student records. This project demonstrates a clear separation of concerns by isolating the database models into a dedicated data app while managing all network traffic and serialization through a centralized API gateway.

## Features
* Full CRUD (Create, Read, Update, Delete) capabilities for Student records.
* Function-based views utilizing DRF `@api_view` decorators.
* Robust data validation via DRF ModelSerializers.
* Browsable API interface for easy testing.

## Tech Stack
* **Language:** Python
* **Framework:** Django, Django REST Framework
* **Database:** SQLite (Development)

## API Endpoints
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/v1/students/` | Returns a list of all students. |
| `POST` | `/api/v1/students/` | Creates a new student record. |

## Setup and Installation
1. Clone the repository
2. Create and activate a virtual environment:
   `python -m venv env`
   `source env/bin/activate` # (Or `env\Scripts\activate` on Windows)
3. Install dependencies:
   `pip install django djangorestframework`
4. Apply migrations:
   `python manage.py migrate`
5. Run the development server:
   `python manage.py runserver`
