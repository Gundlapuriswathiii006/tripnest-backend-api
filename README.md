# TripNest – Node.js & Express REST API

TripNest is a backend RESTful API built using Node.js and Express.js for managing travel trips.  
This project focuses on backend development and API design and is fully tested using Postman.

Frontend is not included in this repository.

---

## Features

- Create a new trip
- Get all trips
- Get trip by ID
- Update trip details
- Delete trip
- RESTful API architecture
- Proper HTTP status codes

---

## 🔐 Authentication & Authorization (JWT)

This API uses **JSON Web Tokens (JWT)** for secure authentication and authorization.

- Users authenticate using email and password.
- On successful login, a JWT token is generated.
- The token must be sent in the request headers to access protected routes.

---

## Authorization:

- Token verification is handled using middleware.
- Requests with missing or invalid tokens are rejected.

---

## 🛡 Protected Routes

- Sensitive API endpoints are protected using JWT authentication.
- Only authenticated users can access protected resources.
- Unauthorized access returns appropriate HTTP status codes.

---

## 👮 Role-Based Access Control (Admin)

- The application supports **Admin and User roles**.
- Role validation is performed after JWT verification.

**Admin users can:**
- Create trips
- Update trips
- Delete trips

**Normal users can:**
- View trips only
- book trips and view bookings

- Admin-only routes are restricted and secured.

---

## 🧪 API Testing (Postman)

- All APIs were tested using **Postman**.
- JWT tokens were generated and attached to request headers.
- Admin and user access were verified successfully.

## Tech Stack

- Node.js
- Express.js
- MongoDB
- Postman
- Git & GitHub

---

## Project Structure

tripnest-node-express-api
│
├── controllers
├── routes
├── models
├── screenshots
│
├── server.js
├── package.json
└── README.md

---

## API Endpoints

POST    /api/trips/create       → Create a trip  
GET     /api/trips/my-trips       → Get all trips  
GET     /api/trips/:id    → Get trip by ID  
PUT     /api/trips/:id    → Update trip  
DELETE  /api/trips/:id    → Delete trip  

---

## Postman Testing

All APIs have been tested using Postman.

the screenshots are added to folder.

---

## Run the Project  
cd tripnest-node-express-api  
npm install  
npm start  

Server runs on:  
http://localhost:4000

---

## Learning Outcomes

- Built REST APIs using Express.js
- Implemented CRUD operations
- Understood backend routing and controllers
- Practiced API testing using Postman
- Improved GitHub workflow

---

## Author

Gundlapuri Swathi  
B.Tech – Computer Science and Engineering
