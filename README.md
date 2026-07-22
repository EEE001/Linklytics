# Linklytics

A modern full-stack URL shortening and analytics platform built with **Spring Boot**, **React**, and **MySQL**.

Linklytics allows users to create shortened URLs, manage their links, and analyze visitor traffic through detailed click analytics. The project is designed with scalability, security, and clean architecture in mind while following modern backend and frontend development practices.

---

# Features

## Authentication

- User Registration
- User Login
- JWT Authentication
- Password Encryption (BCrypt)
- Protected API Endpoints
- Spring Security Integration

---

## URL Management

- Create Short URLs
- Redirect Short URLs
- View User URLs
- Delete URLs
- Unique Short Code Generation

---

## Analytics

- Click Tracking
- Click Counter
- Click History
- Timestamp Logging
- Visitor Statistics
- URL Performance Dashboard *(Upcoming)*

---

## Security

- JWT Token Authentication
- Stateless Authentication
- Password Hashing
- Protected REST APIs
- Spring Security Filter Chain

---

# Tech Stack

## Backend

- Java 17
- Spring Boot 3
- Spring Security
- Spring Data JPA
- Hibernate
- JWT
- Maven

## Frontend

- React
- Vite
- Tailwind CSS *(planned)*
- Axios
- React Router

## Database

- MySQL

---

# Project Structure

```
Linklytics/
│
├── backend/
│   ├── src/
│   ├── pom.xml
│   ├── mvnw
│   └── ...
│
├── frontend/
│
└── README.md
```

---

# Architecture

```
React Frontend
       │
       ▼
Spring Boot REST API
       │
       ▼
Spring Security
       │
       ▼
Business Services
       │
       ▼
Spring Data JPA
       │
       ▼
MySQL Database
```

---

# Backend Modules

```
controller/
    REST API Endpoints

service/
    Business Logic

repository/
    Database Access

models/
    Entity Classes

dtos/
    Request & Response DTOs

security/
    JWT Authentication
    Spring Security Configuration
```

---

# API Endpoints

## Authentication

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/auth/register | Register User |
| POST | /api/auth/login | Login User |

---

## URL

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/url | Create URL |
| GET | /api/url | Get User URLs |
| DELETE | /api/url/{id} | Delete URL |

---

## Redirect

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /{shortUrl} | Redirect to Original URL |

---

# Getting Started

## Clone Repository

```bash
git clone https://github.com/EEE001/Linklytics.git
```

---

## Backend Setup

```bash
cd backend
```

### Configure Environment Variables

Set the following variables:

```
DB_URL
DB_USERNAME
DB_PASSWORD
JWT_SECRET
```

Example:

```
DB_URL=jdbc:mysql://localhost:3306/urlshortnerdb
DB_USERNAME=root
DB_PASSWORD=your_password
JWT_SECRET=your_secret_key
```

---

### Build Project

```bash
./mvnw clean install
```

or on Windows

```powershell
mvnw.cmd clean install
```

---

### Run Backend

```bash
./mvnw spring-boot:run
```

---

## Frontend Setup

```bash
cd frontend
```

Install dependencies

```bash
npm install
```

Run development server

```bash
npm run dev
```

---

# Database

Current database:

```
MySQL
```

Tables

- users
- url_mapping
- click_event

---

# Current Progress

## Backend

- [x] JWT Authentication
- [x] User Registration
- [x] User Login
- [x] URL Shortening
- [x] URL Redirection
- [x] Click Tracking
- [x] MySQL Integration

## Frontend

- [ ] Authentication UI
- [ ] Dashboard
- [ ] URL Management
- [ ] Analytics Dashboard
- [ ] Charts
- [ ] Responsive Design

---

# Future Improvements

- QR Code Generation
- Custom Short URLs
- URL Expiration
- Rate Limiting
- Redis Cache
- Docker Support
- Kubernetes Deployment
- CI/CD with GitHub Actions
- Email Verification
- Password Reset
- Admin Dashboard
- Geographic Analytics
- Device Analytics

---

# Screenshots

*(Will be added after frontend implementation.)*

---

# Author

**Emon Ghosh**

GitHub: https://github.com/EEE001

Feel free to connect or explore my other projects on GitHub.

GitHub:
https://github.com/EEE001
