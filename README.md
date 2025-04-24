# Farm Stack App

A FastAPI-based web application with automatic API documentation.

FARM stands for FAstAPI - Backend, React - Frontend, MongoDB-Database

## Features

- FastAPI framework with automatic API documentation
- Swagger UI available at `/docs`
- ReDoc available at `/redoc`
- Python virtual environment setup
- Type hints and data validation with Pydantic

## Prerequisites

- Python 3.13.2 or higher
- pip (Python package installer)

## Setup Instructions

1. Clone the repository:
```bash
git clone <repository-url>
cd farm-stack-app
```

2. Create and activate a virtual environment:
```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
# On macOS:
source venv/bin/activate
# On Windows:
# venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install "fastapi[standard]"
```

4. Run the application:
```bash
uvicorn main:app --reload
```

The application will be available at `http://127.0.0.1:8000`

## API Documentation

FastAPI automatically generates interactive API documentation:

- Swagger UI: `http://127.0.0.1:8000/docs`
- ReDoc: `http://127.0.0.1:8000/redoc`

## Project Structure

```
farm-stack-app/
├── venv/                  # Virtual environment
├── main.py               # Main application file
└── README.md            # This file
```

## API Endpoints

- `GET /`: Returns a hello world message
- `GET /items/{item_id}`: Get item by ID
- `PUT /items/{item_id}`: Update item by ID

## Development

The application uses hot-reload, so any changes to the code will automatically restart the server.

## Resources

- [FastAPI Documentation](https://fastapi.tiangolo.com/)
- [Tutorial Video](https://www.youtube.com/watch?v=PWG7NlUDVaA) 