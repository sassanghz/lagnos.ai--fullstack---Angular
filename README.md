**Lagnos Web Application**
This project is a web application that includes:

A Spring Boot backend for handling user authentication and database interactions using SQLite.
A frontend application (Angular) for user interaction, allowing users to login and perform actions on the website.

To run this project, you need to have:

Java 11 or higher installed for the backend.
Node.js and npm installed for the frontend (if you're using Angular or React).
SQLite installed or included in the project dependencies.


git clone https://github.com/sassanghz/lagnos.ai--Springboot-Angular.git
cd lagnos-backend

You can start the backend server with the following command:

bash
Copy code
./mvnw spring-boot:run  # For Windows, use .\mvnw.cmd spring-boot:run

The server should start on http://localhost:8080

Verify Backend:

You can use Postman or similar API client to test the login endpoint:

Endpoint: POST http://localhost:8080/api/users/login
Body:
json
Copy code
{
  "email": "sassi@gmail.com",
  "password": "qwe"
}

Navigate to the Frontend Directory:

bash
Copy code
cd ../lagnos-frontend  

Run the Frontend Application:
ng serve   # For Angular

By default, Angular will start on http://localhost:4200

Troubleshooting
Backend Issues:

Ensure that Java and Maven are installed correctly.
If the database is missing, check that schema.sql is in src/main/resources and that spring.datasource.initialization-mode=always is set in application.properties.
Frontend Issues:

Check that the frontend server URL matches the backend’s base URL.
If npm install fails, make sure Node.js and npm are up-to-date.


