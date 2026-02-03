# ✈️ Airline Booking System (Microservices Based – Backend)

A backend-only **Airline Booking System** built using **Node.js, Express, MySQL, and Sequelize** following **Microservices Architecture**.

This project provides RESTful APIs for searching, managing, and booking flights.  
It is designed to be consumed by any frontend (Web / Mobile).

Built with focus on **scalability, security, and clean architecture**.

---

## 🌐 Architecture Overview

This system is divided into multiple independent microservices:

| Service | Description | Repository |
|---------|-------------|------------|
| Auth Service | Authentication & JWT | [[[[[https://github.com/your-username/auth-service](https://github.com/ravikumar9555/AUTHSERVICE)](https://github.com/ravikumar9555/AUTHSERVICE.git)]](https://github.com/ravikumar9555/AUTHSERVICE.git)(https://github.com/ravikumar9555/AUTHSERVICE.git)](https://github.com/ravikumar9555/AUTHSERVICE) |
| Flight Service | Flight Search & Management |[ https://github.com/your-username/flight-service](https://github.com/ravikumar9555/FLIGHTSANDSERACHSERVICE) |
| Booking Service | Booking Management | [https://github.com/your-username/booking-service](https://github.com/ravikumar9555/BOOKINGSERVICE) |

> ⚠️ Replace links with your real GitHub repositories.

---

## 📌 Key Features

### 🔐 Authentication
- JWT-based login & registration
- Token validation on every request
- Auto logout on token expiry
- Role-based access (ADMIN / CUSTOMER)

---

### ✈️ Flight Management
- Create / Update / Delete flights
- Search flights with advanced filters
- Price, date, seat, and route filtering
- Pagination support

---

### 🏢 Airport & City Management
- Add / update airports
- Add / update cities
- City → Airport mapping
- Validation and referential integrity

---

### 🛫 Airplane Management
- Manage airplanes
- Capacity validation
- Automatic seat handling

---

### 📦 Booking System
- Create bookings
- Seat availability validation
- Booking history
- Secure booking flow

---

### 🔍 Advanced Search
- City-based search
- Multi-airport filtering
- Date range filtering
- Seat availability
- Price range filtering
- Backend optimized Sequelize queries

---

### 🔒 Security
- JWT Authorization
- Protected APIs
- Middleware validation
- Request sanitization
- Unauthorized access blocking

---

## 🏗️ Tech Stack

### Backend
- Node.js
- Express.js
- Sequelize ORM
- JWT Authentication
- REST API

### Database
- MySQL

---

## 📂 Microservices Design

Each service contains:

- Independent database models
- Dedicated API routes
- Service-specific business logic
- Separate deployment capability


---

## 🗄️ Database Schema

### Users
| Field | Type |
|-------|------|
| id | INT |
| email | VARCHAR |
| password | VARCHAR |
| role | ENUM |

---

### Airplanes
| Field | Type |
|-------|------|
| id | INT |
| modelNumber | VARCHAR |
| capacity | INT |

---

### Airports
| Field | Type |
|-------|------|
| id | INT |
| name | VARCHAR |
| cityId | INT |

---

### Cities
| Field | Type |
|-------|------|
| id | INT |
| name | VARCHAR |

---

### Flights
| Field | Type |
|-------|------|
| id | INT |
| flightNumber | VARCHAR |
| airplaneId | INT |
| departureAirportId | INT |
| arrivalAirportId | INT |
| departureTime | DATETIME |
| arrivalTime | DATETIME |
| price | INT |
| totalSeats | INT |

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repositories

```bash
git clone https://github.com/your-username/auth-service
git clone https://github.com/your-username/flight-service
git clone https://github.com/your-username/airport-service
git clone https://github.com/your-username/booking-service
