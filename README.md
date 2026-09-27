# FundooNotes

## 📌 Project Overview

FundooNotes is a **Spring Boot based Notes Management System** designed to provide secure and organized management of personal notes.

The application allows users to register and authenticate securely, create and manage notes, organize notes using labels, set reminders, and manage attachments.

The project also demonstrates the use of **Spring Security, JWT authentication, Redis, JMS messaging, Spring Data JPA, Spring AOP, and OpenAPI/Swagger** in a real-world backend application.

---

## 🚀 Features

### 👤 User Management

- User registration
- User login
- JWT-based authentication
- Password reset functionality
- Secure API access using Spring Security

### 📝 Notes Management

Users can:

- Create notes
- View notes
- Update notes
- Delete notes
- Manage note details
- Organize notes using labels
- Set reminders for notes
- Add attachments to notes

### 🏷️ Label Management

- Create labels
- View labels
- Update labels
- Delete labels
- Associate labels with notes

### ⏰ Reminder Management

- Create reminders
- View reminders
- Update reminders
- Delete reminders
- Associate reminders with notes

### 📎 Attachment Management

- Add attachments to notes
- Retrieve attachments
- Manage note attachments

### 🔐 Security

The application uses:

- Spring Security
- JWT authentication
- JWT authentication filter
- Custom security configuration
- Token validation

### ⚡ Redis

Redis is used for token-related caching and management.

### 📨 JMS Messaging

JMS with Artemis is used for asynchronous notification messaging.

The project contains:

- Notification Producer
- Notification Consumer
- JMS configuration

### 📊 Logging

Spring AOP is used to implement application logging through an aspect-oriented approach.

### 📖 API Documentation

OpenAPI / Swagger configuration is included for API documentation and testing.

### 🌐 CORS

CORS configuration is provided to allow controlled communication between the backend and frontend applications.

### ⚠️ Exception Handling

The application provides centralized exception handling using a global exception handler.

Custom exceptions are used for situations such as:

- User not found
- Note not found
- Label not found
- Reminder not found
- Attachment not found
- Duplicate email
- Invalid password
- Invalid token

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Java | Programming language |
| Spring Boot | Application framework |
| Spring MVC | REST API development |
| Spring Data JPA | Database persistence |
| Spring Security | Application security |
| JWT | Authentication |
| PostgreSQL | Database |
| Redis | Token caching |
| JMS | Messaging |
| Artemis | Message broker |
| Maven | Build and dependency management |
| Spring AOP | Logging |
| OpenAPI / Swagger | API documentation |

---

## 🏗️ Project Architecture

The project follows a layered architecture:

```text
                    Client
                       |
                       v
                +--------------+
                | Controllers  |
                +--------------+
                       |
                       v
                +--------------+
                |   Services   |
                +--------------+
                       |
                       v
                +--------------+
                | Repositories  |
                +--------------+
                       |
                       v
                   Database
