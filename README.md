# Task Management API

A REST API built with Python and FastAPI for managing tasks.

## Overview

This project was developed as a personal software engineering portfolio project.

The API provides endpoints to create, retrieve, update, and delete tasks using standard HTTP methods.

## Technologies

- Python
- FastAPI
- Uvicorn
- Pydantic
- Pytest
- REST API
- JSON
- Git
- GitHub

## Features

- Create tasks
- List all tasks
- Retrieve a task by ID
- Update tasks
- Delete tasks
- Input validation
- HTTP status codes
- Automated tests
- Interactive API documentation

## Project Structure

```text
task-management-api/
├── app/
│   ├── __init__.py
│   └── main.py
├── tests/
│   └── test_main.py
├── .gitignore
├── README.md
└── requirements.txt
```

## Installation

Clone the repository:

```bash
git clone https://github.com/Cirlenemaciel/task-management-api.git
```

Navigate to the project directory:

```bash
cd task-management-api
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

On Linux or macOS:

```bash
source venv/bin/activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

## Running the API

Start the development server:

```bash
uvicorn app.main:app --reload
```

The API will be available at:

```text
http://127.0.0.1:8000
```

## API Documentation

FastAPI automatically provides interactive API documentation.

### Swagger UI

```text
http://127.0.0.1:8000/docs
```

### ReDoc

```text
http://127.0.0.1:8000/redoc
```

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/` | Check API status |
| GET | `/tasks` | Get all tasks |
| GET | `/tasks/{id}` | Get a task by ID |
| POST | `/tasks` | Create a new task |
| PUT | `/tasks/{id}` | Update a task |
| DELETE | `/tasks/{id}` | Delete a task |

## Example Request

Create a new task:

```json
{
  "title": "Learn Python",
  "description": "Study Python fundamentals",
  "completed": false
}
```

## Example Response

```json
{
  "id": 1,
  "title": "Learn Python",
  "description": "Study Python fundamentals",
  "completed": false
}
```

## Running Tests

Run the automated test suite with:

```bash
pytest
```

## Future Improvements

Possible improvements for future versions:

- PostgreSQL database
- User authentication
- JWT authentication
- Docker support
- Pagination
- Search and filtering
- Frontend interface
- CI/CD with GitHub Actions
- Environment variable configuration
- Database migrations

## Author

**Cirlene Maciel**

Junior Software Engineer | Python | JavaScript | Automation | AI
