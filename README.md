#  Fitness Tracker – MERN Capstone Project

A full-stack fitness tracking application built with the MERN stack. Users can register, log in, and manage their workout sessions through a clean, responsive dashboard.

---

##  Features

-  **User Authentication** using JWT and bcrypt
-  **Workout Logging** – track type, duration, calories, and notes
-  **Workout History** – view your past sessions
-  (Optional) **Real-Time Updates** with Socket.io
-  **Fully Responsive Design**
-  **Deployed** on Vercel (frontend) and Render (backend)

---

##  Tech Stack

| Layer      | Tech               |
|------------|--------------------|
| Frontend   | React, Axios, Tailwind CSS |
| Backend    | Node.js, Express.js |
| Database   | MongoDB Atlas      |
| Auth       | JWT, bcrypt        |
| Deployment | Vercel (frontend), Render (backend) |

---

##  API Endpoints

POST /api/auth/register # Register a new user
POST /api/auth/login # Login and receive token
GET /api/workouts # Get user's workouts (token required)
POST /api/workouts # Create a new workout
GET /api/workouts/:id # Get one workout
PUT /api/workouts/:id # Update a workout
DELETE /api/workouts/:id # Delete a workout



> All `/workouts` routes require an `Authorization: Bearer <token>` header.

---

## 🖥 Screenshots

| Login/Register | Dashboard | Add Workout |
|----------------|-----------|-------------|
| ![Login](./screenshots/login.png) | ![Dashboard](./screenshots/dashboard.png) | ![Add Workout](./screenshots/add.png) |



---

##  Setup Instructions

###  Environment Variables

Create a `.env` file in both `/frontend` and `/backend` folders.

#### `.env` (Backend):
```env
PORT=5000
MONGO_URI=your_mongodb_atlas_url
JWT_SECRET=your_jwt_secret
.env (Frontend):

VITE_API_URL=https://your-backend-url.onrender.com/api
 Local Development


# Setup backend
cd backend
npm install
npm run dev

# Setup frontend
cd ../frontend
npm install
npm run dev
 Deployment
Frontend: https://fitness-tracker.vercel.app

Backend: https://fitness-tracker-api.onrender.com

 Pitch Deck
🖥 Click to view presentation slides https://www.canva.com/design/DAGuLM9zghE/RYs1g7uVYXrwsFgM1X8wfA/edit
