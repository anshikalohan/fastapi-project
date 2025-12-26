# FastAPI User Management System

A secure backend REST API built with **FastAPI**, featuring user authentication, JWT-based authorization, and full CRUD functionality.

---

## Features

- User Signup & Login
- Password Hashing using bcrypt
- JWT Authentication
- Protected Routes
- Full CRUD Operations
- SQLite Database
- Swagger UI for API Documentation

---

## Tech Stack

- **Backend:** FastAPI (Python)
- **Database:** SQLite
- **ORM:** SQLAlchemy
- **Authentication:** JWT (python-jose)
- **Security:** Passlib (bcrypt)
- **Server:** Uvicorn

---

## Project Structure

```
fastapi_project/
│
├── app/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── schemas.py
│   ├── auth.py
│   ├── security.py
│
├── requirements.txt
└── README.md
```

---

## Setup Instructions

### Clone the repository

```bash
git clone <https://github.com/anshikalohan/fastapi-project>
cd fastapi_project
```

### Create virtual environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the server

```bash
uvicorn app.main:app --reload
```

---

## API Documentation

Once the server is running, open:

 **http://127.0.0.1:8000/docs**

Swagger UI allows you to test all endpoints interactively.

---

## Authentication Flow

1. User signs up
2. User logs in
3. Server returns JWT token
4. Token is sent in `Authorization: Bearer <token>`
5. Protected routes verify token using dependencies

---

## Endpoints Overview

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/signup` | Register user |
| POST | `/login` | Login user |
| GET | `/users` | Get all users |
| GET | `/me` | Get logged-in user |

---

## Learning Outcomes

- Built a production-style backend using FastAPI
- Implemented secure authentication and authorization
- Gained hands-on experience with ORMs and JWT
- Followed clean architecture and REST best practices

---

## Author

**Anshika**  
B.Tech Student | Backend Development | FastAPI
