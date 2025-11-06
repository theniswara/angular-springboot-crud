# Angular + Spring Boot CRUD Application

This project is a full-stack CRUD web application built with **Angular** (frontend) and **Spring Boot** (backend).  
It demonstrates how to connect an Angular client with a Spring Boot REST API using MySQL as the database.

---

## 🧩 Project Structure

Angular-10-Spring-Boot-CRUD-Full-Stack-App/
├── angular-frontend/ # Frontend (Angular)
└── springboot-backend/ # Backend (Spring Boot)

yaml
Copy code

---

## ⚙️ Backend Setup (Spring Boot)

1. Open the project folder:
   ```bash
   cd springboot-backend
Open src/main/resources/application.properties
Update the following fields with your local MySQL credentials:

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/YOUR_DATABASE_NAME
spring.datasource.username=YOUR_DB_USERNAME
spring.datasource.password=YOUR_DB_PASSWORD
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
Run the backend using IntelliJ IDEA or command line:

bash
Copy code
./mvnw spring-boot:run
The backend runs on: http://localhost:8080

💻 Frontend Setup (Angular)
Open a new terminal and go to the frontend directory:

bash
Copy code
cd angular-frontend
Install dependencies:

bash
Copy code
npm install
Run the Angular development server:

bash
Copy code
ng serve
The frontend runs on: http://localhost:4200

Make sure the backend is running before using the frontend.

🔐 Security Notice
Do not commit your real database credentials.

Before committing:

Replace your username and password in application.properties with placeholders:

properties
Copy code
spring.datasource.username=YOUR_DB_USERNAME
spring.datasource.password=YOUR_DB_PASSWORD
Then add the file to .gitignore so it won’t be pushed again:

css
Copy code
/springboot-backend/src/main/resources/application.properties
🚀 Running the Application
Start the backend server:

bash
Copy code
cd springboot-backend
./mvnw spring-boot:run
Start the frontend:

bash
Copy code
cd angular-frontend
ng serve
Open the browser and navigate to:

arduino
Copy code
http://localhost:4200
🧱 Tech Stack
Frontend: Angular

Backend: Spring Boot

Database: MySQL

Build Tools: Maven, Node.js

📄 License
This project is open source and available for educational purposes.

yaml
Copy code

---
