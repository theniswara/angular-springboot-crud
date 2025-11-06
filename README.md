# Campus Web App

A full-stack web application built with **Angular** (frontend) and **Spring Boot** (backend).  
This project is designed to manage campus-related features such as lecturer data, students, announcements, and AI chatbot integration.

---

## 🚀 Tech Stack

**Frontend:** Angular  
**Backend:** Spring Boot  
**Database:** MySQL  
**API Testing:** Postman (optional)

---

## 🧩 Project Structure

root/
├── backend/ # Spring Boot project
│ ├── src/main/java
│ ├── src/main/resources
│ └── pom.xml
│
└── frontend/ # Angular project
├── src/
├── angular.json
└── package.json

yaml
Copy code

---

## ⚙️ Prerequisites

Make sure you have the following installed:

- **Node.js** (v16 or higher)
- **Angular CLI** (`npm install -g @angular/cli`)
- **Java JDK 17+**
- **Maven**
- **MySQL Server**

---

## 🗄️ Database Setup

1. Create a new MySQL database:
   ```sql
   CREATE DATABASE campus_webapp;
Update your application.properties (in Spring Boot) with:

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/campus_webapp
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
▶️ Running the Project
1. Backend (Spring Boot)
bash
Copy code
cd backend
mvn spring-boot:run
Backend will start on:

arduino
Copy code
http://localhost:8080
2. Frontend (Angular)
bash
Copy code
cd frontend
npm install
ng serve
Frontend will start on:

arduino
Copy code
http://localhost:4200
🌐 Connecting Frontend and Backend
In your Angular environment file (environment.ts), set your API URL:

typescript
Copy code
export const environment = {
  production: false,
  apiUrl: 'http://localhost:8080/api'
};
🧪 API Testing (Optional)
Use Postman to test backend APIs before connecting to Angular.

Example:

bash
Copy code
GET http://localhost:8080/api/employees
👥 Team Members
Name	Role
Member 1	Frontend Developer
Member 2	Backend Developer
Member 3	Database & API Integration
Member 4	UI/UX & Documentation

📄 License
This project is for educational purposes only.

💡 Notes
Make sure both backend and frontend servers are running before testing.

For production, build Angular with:

bash
Copy code
ng build --prod
and deploy the generated dist/ folder inside Spring Boot’s static/ directory if needed.
