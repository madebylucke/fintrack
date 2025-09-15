# Fintrack
FinTrack is a mock digital banking platform built in Java (Spring Boot + PostgreSQL).
It simulates the core features of modern banking systems, showcasing how real-world financial backends handle users, transactions, and fraud detection.

This project demonstrates strong backend engineering, database design, and enterprise-level development practices.

## ✨ Features

- **User Management**
  - JWT-based authentication (signup/login)
  - Role-based access (customer/admin)

- **Accounts**
  - Multiple account types per user (checking, savings)
  - Real-time balance tracking

- **Transactions**
  - Transfer money between accounts
  - Deposit & withdrawal operations
  - Transaction history with filtering and pagination

- **Fraud Detection**
  - Rule-based alerts for unusual transactions
  - Admin endpoint for monitoring flagged activity

- **API Documentation**
  - Swagger UI for interactive API exploration

## 🛠️ Tech Stack

- **Java 21** – Core backend logic  
- **Spring Boot 3** – REST API framework  
- **Spring Security + JWT** – Authentication & authorization  
- **Hibernate (JPA)** – ORM for PostgreSQL  
- **PostgreSQL** – Database  
- **Swagger/OpenAPI** – API documentation  
- **Docker** – Containerized deployment 

## 🔗 API Endpoints

**Authentication**
- `POST /auth/signup` → Create account  
- `POST /auth/login` → Get JWT token  

**Accounts**
- `GET /accounts` → List user accounts  
- `POST /accounts` → Create new account  

**Transactions**
- `POST /transactions` → Transfer money  
- `GET /transactions` → View transaction history  

**Admin**
- `GET /admin/users` → List all users  
- `GET /admin/fraud-alerts` → View flagged transactions 

## 📌 Getting Started

**Clone & Run:**

```bash
git clone https://github.com/madebylucke/fintrack.git
cd fintrack
./mvnw spring-boot:run
