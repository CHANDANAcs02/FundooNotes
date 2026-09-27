# FundooNotes

## Project Overview

FundooNotes is a Spring Boot based **Notes Management Application** that allows users to register, login, create and manage notes, labels, reminders, and attachments.

The application provides secure authentication using **JWT**, stores data using **Spring Data JPA**, and uses **Redis and JMS messaging** for additional services.

## What the Project Does

The application provides the following features:

- User registration and login
- JWT-based authentication
- Create, update, view and delete notes
- Create and manage labels
- Add labels to notes
- Create and manage reminders
- Add attachments to notes
- Password reset functionality
- Redis-based token management
- JMS-based notification messaging
- Global exception handling
- API documentation using OpenAPI / Swagger
- CORS configuration
- Logging using Spring AOP

## Technologies Used

- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Spring Security
- JWT
- MySQL
- Redis
- JMS / Artemis
- Maven
- OpenAPI / Swagger
- Spring AOP

## Project Structure

src/main/java/com/bridgelabz/fundoo/notes
│
├── aspect
├── config
├── controller
├── dto
├── entity
├── exception
├── jms
├── redis
├── repository
├── security
└── service

**Main Modules**
Authentication
User registration
User login
JWT token generation and validation
Password reset
Notes
Create notes
Update notes
View notes
Delete notes
Labels
Create labels
Update labels
Delete labels
Manage labels for notes
Reminders
Create reminders
Update reminders
Delete reminders
Attachments
Add attachments
Retrieve attachments
Manage note attachments
Security

The application uses Spring Security and JWT authentication to protect secured APIs.

**Messaging**

JMS and Artemis are used for notification messaging between application components.

**Redis**

Redis is used for token caching and token management.

**API Documentation**

OpenAPI / Swagger is configured to provide interactive API documentation.

**Architecture**

The project follows a layered architecture:

Controller
    ↓
Service
    ↓
Repository
    ↓
Database

Supporting components such as Security, Redis, JMS, AOP, and Exception Handling are integrated into the application.

**How to Run**
Clone the repository.
Configure the database in application.properties.
Configure Redis and Artemis if required.
Build the project using Maven.
Run the Spring Boot application.
mvn spring-boot:run
Purpose

The project demonstrates the development of a real-world Spring Boot application using:

REST APIs
Authentication and Authorization
Database persistence
JWT Security
Redis
JMS Messaging
Exception Handling
AOP Logging
OpenAPI Documentation
