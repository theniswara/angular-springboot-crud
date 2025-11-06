# Angular + Spring Boot CRUD Application

This project is a full-stack CRUD web application built with **Angular** (frontend) and **Spring Boot** (backend).  
It demonstrates how to connect an Angular client with a Spring Boot REST API using MySQL as the database.

---

## 🧩 Project Structure

Angular-10-Spring-Boot-CRUD-Full-Stack-App/  
├── angular-frontend/ # Frontend (Angular)  
└── springboot-backend/ # Backend (Spring Boot)

---

## ⚙️ Backend Setup (Spring Boot)

1. Open the project folder:
   ```bash
   cd springboot-backend

2. Open `src/main/resources/application.properties` and update the following fields with your local MySQL credentials:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/YOUR_DATABASE_NAME
   spring.datasource.username=YOUR_DB_USERNAME
   spring.datasource.password=YOUR_DB_PASSWORD
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.show-sql=true
   spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
   ```

3. Run the backend using IntelliJ IDEA or command line:

   ```bash
   ./mvnw spring-boot:run
   ```

The backend runs on: **[http://localhost:8080](http://localhost:8080)**

---

## 💻 Frontend Setup (Angular)

1. Open a new terminal and go to the frontend directory:

   ```bash
   cd angular-frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Run the Angular development server:

   ```bash
   ng serve
   ```

The frontend runs on: **[http://localhost:4200](http://localhost:4200)**

> Make sure the backend is running before using the frontend.

---

## 🔐 Security Notice

Do not commit your real database credentials.

Before committing, replace your username and password in `application.properties` with placeholders:

```properties
spring.datasource.username=YOUR_DB_USERNAME
spring.datasource.password=YOUR_DB_PASSWORD
```

Then add the file to `.gitignore` so it won’t be pushed again:

```bash
/springboot-backend/src/main/resources/application.properties
```

---

## 🚀 Running the Application

Start the backend server:

```bash
cd springboot-backend
./mvnw spring-boot:run
```

Start the frontend:

```bash
cd angular-frontend
ng serve
```

Open the browser and navigate to:

```
http://localhost:4200
```

---

## 🧱 Tech Stack

* Frontend: Angular
* Backend: Spring Boot
* Database: MySQL
* Build Tools: Maven, Node.js

---

## 📄 License

This project is open source and available for educational purposes.

```
```

