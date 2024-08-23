# Running-App
Application to generate customised running routes for users using third-party APIs like Google Maps 

Backend Setup Guide

Introduction
This guide provides detailed instructions for setting up a Python environment for backend using FastAPI, Uvicorn, and several other packages crucial for development, security, and database interaction.

Environment Setup
1. Install Python:
Download Python from python.org and follow the installation instructions for your operating system.
2. Setup Virtual Environment:
Open a terminal or command prompt, navigate to the project directory, and run the following command to create a virtual environment:
python -m venv venv
Activate the virtual environment:
- Windows:
.\venv\Scripts\activate
- macOS/Linux:
source venv/bin/activate
3. Install Required Packages:
Ensure your virtual environment is activated and install the necessary Python packages using pip:
pip install fastapi uvicorn pymongo "python-bsonjs>=0.2.0" passlib[bcrypt] PyJWT requests python-dotenv
Running the Application
1. Start the Application:
Navigate to the project directory where `main.py` is located and run the application using Uvicorn with the following command:
uvicorn app.main:app --reload
The `--reload` flag enables auto-reloading of the server when code changes are made.
2. Accessing the Application:
Open a web browser and go to http://127.0.0.1:8000 to see the running application.

Usage of Packages
- **FastAPI**: For creating RESTful APIs with automatic Swagger documentation.
- **Uvicorn**: ASGI server for hosting FastAPI applications.
- **PyMongo**: MongoDB driver for Python.
- **PyJWT**: For encoding and decoding JWT tokens, used in authentication.
- **Passlib and bcrypt**: For secure password hashing.
- **Requests**: For making HTTP requests to external services.
- **python-dotenv**: For loading environment variables from `.env` file.
