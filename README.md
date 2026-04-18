# Full-Stack-E-Commerce-App-
Full Stack E-Commerce App using Spring Boot &amp; React with Cart, Soft Delete, Restore &amp; Modern UI

# 🛒 MyStore Pro - Full Stack E-Commerce App

A modern full-stack e-commerce application built using **Spring Boot + React** with advanced UI and real-time API integration.

---

## 🚀 Tech Stack

### Backend
- Java 17
- Spring Boot
- Spring Data JPA
- MySQL
- REST APIs

### Frontend
- React.js
- Axios
- Framer Motion (Animations)
- React Icons

---

## ✨ Features

### 🛍 Product Management
- View all products
- Add new products
- Update product details
- Soft delete (not permanently removed)
- Restore deleted products

### 🛒 Cart System
- Add to cart
- Quantity management (+ / -)
- Prevent duplicate entries
- Real-time cart preview

### 🎨 UI Features
- Modern gradient UI
- Glassmorphism cards
- Smooth animations
- Responsive layout

---

## 🔥 API Endpoints

| Method | Endpoint | Description |
|--------|--------|-------------|
| GET | /api/products | Get all products |
| GET | /api/products/{id} | Get product by ID |
| POST | /api/products | Add product |
| PUT | /api/products/{id} | Update product |
| DELETE | /api/products/{id} | Soft delete |
| GET | /api/products/deleted | Get deleted products |
| PUT | /api/products/restore/{id} | Restore product |

---

## 🛠 Setup Instructions

### 1️⃣ Clone Repository
```bash
git clone https://github.com/your-username/mini-ecommerce-app.git

2️⃣ Backend Setup
cd backend
mvn clean install
mvn spring-boot:run

Update application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update

3️⃣ Frontend Setup

cd frontend
npm install
npm start

🗄 Database

CREATE DATABASE ecommerce;

USE ecommerce;

CREATE TABLE product (
  id BIGINT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(255),
  category VARCHAR(255),
  price DOUBLE,
  stock INT,
  deleted BOOLEAN DEFAULT FALSE
);
