
# Student Management REST API

A REST API built using Python and FastAPI to manage student records with a MySQL database.

## Technologies Used
- Python
- FastAPI
- MySQL
- SQLAlchemy
- Pydantic
- Swagger UI

## Features
- Create new student records
- Retrieve all students or a student by ID
- Filter students by course and paginate results
- Update student details using PUT
- Partially update student details using PATCH
- Delete student records
- Validate input data and handle missing student records

## Setup and Installation

1. Clone the repository.
2. Install the required packages:

   ```bash
   python -m pip install -r requirements.txt
   ```

3. Create a `.env` file in the project folder and add your database connection:

   ```env
   DATABASE_URL=mysql+pymysql://root:YOUR_PASSWORD@localhost:3306/student_db
   ```

   Replace `YOUR_PASSWORD` with your local MySQL password. Do not upload the `.env` file.

4. Create the database in MySQL:

   ```sql
   CREATE DATABASE student_db;
   ```

5. Start the application:

   ```bash
   python -m uvicorn test:app --reload
   ```

6. Open the API documentation:

   http://127.0.0.1:8000/docs

## Learning Outcomes
- Building REST APIs with FastAPI
- Connecting Python applications to MySQL using SQLAlchemy
- Validating request data with Pydantic
- Testing API endpoints using Swagger UI
