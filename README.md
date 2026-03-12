# Microservices Assignment

This project demonstrates a **microservices architecture** using Node.js, gRPC, and an API Gateway with a Next.js frontend.

## Architecture

Frontend (Next.js + MUI)
|
v
API Gateway (REST)
|
v
gRPC Communication
/            |             
Auth Service   Product Service   Order Service

The API Gateway exposes REST APIs to the frontend and communicates with backend microservices using **gRPC**.

---

# Repository Structure

```
assignments/
   backend/
      gateway/
      auth-service/
      product-service/
      order-service/
   frontend/
```

### Backend Services

| Service         | Description                             |
| --------------- | --------------------------------------- |
| Gateway         | Entry point for all API requests        |
| Auth Service    | Handles signup/login and authentication |
| Product Service | CRUD operations for products            |
| Order Service   | CRUD operations for orders              |

### Frontend

Next.js application providing:

* Home page
* Sign Up
* Sign In
* Dashboard
* Product management
* Order management

---

# Tech Stack

Backend

* Node.js
* Express
* gRPC
* JWT Authentication

Frontend

* Next.js
* Material UI
* Axios

Infrastructure

* Microservices Architecture
* API Gateway Pattern

---

# Setup Instructions

Clone the parent repository:

```
git clone --recurse-submodules https://github.com/YOUR_USERNAME/assignments
```

If submodules are not cloned:

```
git submodule update --init --recursive
```

---

# Running the Backend

Start services individually:

```
cd backend/auth-service
npm install
npm run dev
```

```
cd backend/product-service
npm install
npm run dev
```

```
cd backend/order-service
npm install
npm run dev
```

```
cd backend/gateway
npm install
npm run dev
```

---

# Running the Frontend

```
cd frontend
npm install
npm run dev
```

Application will run at:

```
http://localhost:3000
```

---

# Application Flow

1. User opens Home Page
2. User can Sign Up or Sign In
3. After authentication user is redirected to Dashboard
4. From Dashboard user can navigate to:

   * Products
   * Orders

Products and Orders support full **CRUD operations**.

---

# Microservices Communication

Frontend → API Gateway (REST)

Gateway → Services (gRPC)

---

# Author

Microservices Assignment Project
