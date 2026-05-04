# Jobs Manager API

A secure RESTful API for managing job applications and job tracking. Built with Node.js, Express.js, MongoDB, and JWT authentication.

## Features

* User Registration & Login
* JWT Authentication
* CRUD Operations for Jobs
* Protected Routes
* MongoDB Database Integration
* Rate Limiting for Security
* Helmet Security Middleware
* XSS Protection
* Swagger API Documentation
* Error Handling Middleware
* Environment Variable Support

---

# Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB with Mongoose
* **Authentication:** JWT (JSON Web Tokens)
* **Security:** Helmet, XSS-Clean, Rate Limiter
* **API Documentation:** Swagger UI

---
 

# Installation

## 1. Clone the Repository

```bash
git clone https://github.com/optimus-prime-333/Jobs-Manager/tree/main
```

## 2. Navigate to Project Directory

```bash
cd jobs-manager
```

## 3. Install Dependencies

```bash
npm install
```

---

# Environment Variables

Create a `.env` file in the root directory and add the following:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_LIFETIME=1d
```

---

# Running the Project

## Development Mode

```bash
npm start
```

Server will run on:

```bash
http://localhost:5000
```

---

# API Documentation

Swagger documentation is available at:

```bash
http://localhost:5000/api-docs
```

---

# API Endpoints

## Authentication Routes

### Register User

```http
POST /api/v1/auth/register
```

### Login User

```http
POST /api/v1/auth/login
```

---

## Job Routes (Protected)

### Get All Jobs

```http
GET /api/v1/jobs
```

### Create Job

```http
POST /api/v1/jobs
```

### Get Single Job

```http
GET /api/v1/jobs/:id
```

### Update Job

```http
PATCH /api/v1/jobs/:id
```

### Delete Job

```http
DELETE /api/v1/jobs/:id
```

---

# Security Features

* Rate Limiting to prevent abuse
* Helmet for securing HTTP headers
* XSS Protection
* JWT Authentication
* Error Handling Middleware

---

# Dependencies

Main packages used in the project:

* express
* mongoose
* jsonwebtoken
* bcryptjs
* dotenv
* cors
* helmet
* xss-clean
* express-rate-limit
* swagger-ui-express
* yamljs

---
 

# Future Improvements
 
* Add Docker Support

---
 
