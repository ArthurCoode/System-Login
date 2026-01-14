# 🔐 LoginRegister Authentication API

This project is a **Login and Register Authentication API** built with **Spring Boot**, using **Spring Security** and **JWT (JSON Web Token)** to provide secure authentication and authorization.

It implements a complete authentication flow following modern **REST API** and **security best practices**, making it ideal for **learning purposes** and **developer portfolio projects**.

---

## 🚀 Technologies Used

- Java 17+
- Spring Boot
- Spring Security
- JWT (JSON Web Token)
- Spring Data JPA
- Hibernate
- Lombok
- Maven
- Database: H2 / PostgreSQL / MySQL

---

## 🔑 Features

- ✅ User registration (Register)
- ✅ User authentication (Login)
- ✅ JWT token generation
- ✅ Token validation on protected endpoints
- ✅ Password encryption with BCrypt
- ✅ Stateless authentication
- ✅ RESTful API architecture

---

## 🧠 Concepts Applied

- Token-based authentication (JWT)
- Spring Security filters
- BCrypt password encoder
- DTOs for request and response handling
- Layered architecture (Controller, Service, Repository)
- Secure API design principles

---

## 📂 Project Structure

```bash
src/main/java
 └── com.example.LoginNext
     ├── controllers
     ├── domain.user
     ├── dto
     ├── infra.security
     └── repositories

📌 API Endpoints
🔐 Authentication
Method	Endpoint	Description
POST	/auth/register	Register a new user
POST	/auth/login	Authenticate user and return JWT

📝 Request Examples
🔹 Register
POST /auth/register

json
Copy code
{
  "name": "Arthur",
  "email": "arthur@email.com",
  "password": "123456"
}
🔹 Login
POST /auth/login

json
Copy code
{
  "email": "arthur@email.com",
  "password": "123456"
}
Response

json
Copy code
{
  "token": "eyJhbGciOiJIUzI1NiJ9..."
}

▶️ How to Run the Project
Clone the repository:

git clone https://github.com/ArthurCoode/System-Login.git

Navigate to the project directory:
cd System-Login

Run the application:
mvn spring-boot:run

The API will be available at:
http://localhost:8080
