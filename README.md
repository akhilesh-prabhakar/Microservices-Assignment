# Microservices Assignment

This project demonstrates a **Node.js microservices architecture** using an **API Gateway + gRPC communication** with a **Next.js frontend**.

---

# Architecture

```
Frontend (Next.js + MUI)
        |
        v
API Gateway (REST + Auth)
        |
        v
gRPC Communication
   /              \
Product Service   Order Service
```

The **API Gateway** handles:

* Authentication (Signup/Login)
* Request routing
* Communication with backend services via **gRPC**

---

# Repository Structure

```
Microservices-Assignment/
   backend/
      gateway/
      product-service/
      order-service/
   frontend/
```

| Component       | Description                                       |
| --------------- | ------------------------------------------------- |
| Gateway         | Entry point for all API requests + authentication |
| Product Service | CRUD operations for products                      |
| Order Service   | CRUD operations for orders                        |
| Frontend        | Next.js UI for interacting with the system        |

---

# Tech Stack

### Backend

* Node.js
* Express
* gRPC
* JWT Authentication

### Frontend

* Next.js
* Material UI
* Axios

---

# Clone the Project

Clone with submodules:

```
git clone --recurse-submodules https://github.com/YOUR_USERNAME/Microservices-Assignment
```

If already cloned:

```
git submodule update --init --recursive
```

---

# Installation

Install dependencies for each service.

### Product Service

```
cd backend/product-service
npm install
```

### Order Service

```
cd backend/order-service
npm install
```

### Gateway

```
cd backend/gateway
npm install
```

### Frontend

```
cd frontend
npm install
```

---

# Running the Backend Services

Start services in **separate terminals**.

### 1️⃣ Start Product Service

```
cd backend/product-service
npm run dev
```

### 2️⃣ Start Order Service

```
cd backend/order-service
npm run dev
```

### 3️⃣ Start API Gateway

```
cd backend/gateway
npm run dev
```

---

# Running the Frontend

```
cd frontend
npm run dev
```

Application will run at:

```
http://localhost:3000
```

---

# Application Flow

1. User opens **Home Page**
2. User can **Sign Up / Sign In**
3. After login user is redirected to **Dashboard**
4. Dashboard allows navigation to:

   * Products
   * Orders

---

# Features

### Authentication

* User Signup
* User Login
* JWT Authentication

### Products

* Create Product
* View Products
* Update Product
* Delete Product

### Orders

* Create Order
* View Orders
* Update Order
* Delete Order

---

# Microservice Communication

```
Frontend → API Gateway (REST)
Gateway → Product Service (gRPC)
Gateway → Order Service (gRPC)
```

---

# Author

Microservices Assignment
