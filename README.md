#Assignment 1 - Create a simple REST API Webserver

This is a REST API built using python and flask.
It performs basic CRUD Operations on an in-memory list of students.

C = Create
R = READ
U = UPDATE
D = DELETE

# Fetures

- **GET /Students - Fetches all the students
- **POST /students/<id> - Adds a new student
- **PUT /students/<id>** - Update a student by id
- **DELETE /student/<id>** - Deletes a student by id
- **GET /api/v1/healthcheck** - Checks if the server is running/active or not.

# Setup Instructions

Step 1 - 

Clone the repository


'''' bash

git clone https://github.com/chetanboradeone2n/rest_api_webserver.git

cd rest_api_webserver


Step 2 - 

Create an active virtual environment 

python3 -m venv venv
source venv/bin/activate 

Step 3 - 

Install Requirements 

pip install -r requirements.txt 


Step 4 - 

Run the application 

python3 app.py

# The server will start 127.0.0.1:5000


# Example Requests

1. Healthcheck - 

GET /api/v1/healthcheck
Response: {"status": "ok"}

2. Add a Student - 

POST /students
Body:
{
  "name": "John",
  "email": "john@example.com",
  "age": 21
}


3. Update Student - 

PUT /students/1
Body:
{
  "name": "Johnny",
  "email": "johnny@example.com",
  "age": 22
}


4. Delete Student - 

DELETE /students/1


# Project Structure 

student-api/
├── app.py
├── requirements.txt
└── README.md


# Author -
  Chetan Borade
  Github - @chetanboradeone2n
