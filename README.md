# Django REST Framework API

## Overview
A robust, modular backend REST API built with Django and the Django REST Framework (DRF). This project demonstrates a clear separation of concerns by isolating the database models into a dedicated data app while managing all network traffic and serialization through a centralized API gateway. It showcases a progression from standard function-based logic to highly optimized, Object-Oriented architecture.

## Features
* **Full CRUD Capabilities:** Create, Read, Update, and Delete functionality for database records.
* **Architectural Progression:** Implementation of both Function-Based Views (FBVs) and Class-Based Concrete Generic Views (CBVs), demonstrating an understanding of DRY principles and framework optimization.
* **Robust Data Validation:** Inbound and outbound data serialization using DRF `ModelSerializers`.
* **Clean Routing:** App-level URL routing integrated into a master project dispatcher.
* **Browsable API:** Fully interactive web interface provided by DRF for easy endpoint testing.

## Tech Stack
* **Language:** Python
* **Framework:** Django, Django REST Framework
* **Database:** SQLite (Development)

## API Endpoints
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/v1/data/` | Returns a list of all records. |
| `POST` | `/api/v1/data/` | Validates and creates a new record. |
| `GET` | `/api/v1/data/<int:pk>/` | Retrieves a specific record by its Primary Key (ID). |
| `PUT` | `/api/v1/data/<int:pk>/` | Updates a specific record. |
| `DELETE`| `/api/v1/data/<int:pk>/` | Deletes a specific record. |

