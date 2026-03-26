# journal-crud
📘 Journal Management System – REST API
📌 Project Overview

The Journal Management System is a secure RESTful web application developed using Spring Boot that allows users to create, read, update, and delete personal journal entries. The application implements authentication and role-based access control to ensure secure data access.

This project demonstrates backend development skills including REST API design, database integration, and Spring Security implementation.

🚀 Tech Stack
Backend: Spring Boot
Security: Spring Security (Authentication & Authorization)
Persistence: Spring Data JPA / Hibernate
Database: MySQL
Build Tool: Maven
Language: Java 21
🔐 Key Features
User Registration & Login (Secure Authentication)
Role-Based Access Control
CRUD Operations for Journal Entries
Password Encryption using BCrypt
Exception Handling with Global Exception Handler
Transaction Management using @Transactional
RESTful API Architecture
Data Integrity & Validation
🏗️ Architecture

The project follows a Layered Architecture:

Controller → Service → Repository → Database

Controller Layer: Handles HTTP requests
Service Layer: Contains business logic
Repository Layer: Manages database interactions
Entity Layer: Defines JPA entities and relationships
📂 API Endpoints (Sample)
🔑 Authentication
POST /auth/register – Register new user
POST /auth/login – Authenticate user
📖 Journal Management
GET /journals – Get all journals (Authorized user)
GET /journals/{id} – Get journal by ID
POST /journals – Create journal entry
PUT /journals/{id} – Update journal entry
DELETE /journals/{id} – Delete journal entry
🗄️ Database Design
User Entity
id
username
password
role
Journal Entity
id
title
content
createdDate
user (Many-to-One relationship)
