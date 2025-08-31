# Event-Verse

Event-Verse is a full-stack web application for managing events, tickets, sponsors, feedback, and user activities. The project is divided into two main parts: a **backend** (Node.js/Express/MongoDB) and a **frontend** (Vite/React/Tailwind CSS).

---

## Table of Contents
- [Event-Verse](#event-verse)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Tech Stack](#tech-stack)
  - [Project Structure](#project-structure)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
  - [API Overview](#api-overview)
  - [License](#license)

---

## Features
- Event creation, listing, and management
- Ticket booking and management
- Sponsor applications and management
- User authentication and activity tracking
- Feedback system for events

---

## Tech Stack
- **Backend:** Node.js, Express.js, MongoDB, Mongoose
- **Frontend:** React, Vite, Tailwind CSS

---

## Project Structure
```
Event-Verse/
├── backend/
│   ├── config/           # Database configuration
│   ├── controllers/      # Route controllers (events, tickets, users, etc.)
│   ├── middlewares/      # Authentication and other middleware
│   ├── models/           # Mongoose models
│   ├── routes/           # Express route definitions
│   ├── package.json      # Backend dependencies
│   └── server.js         # Entry point for backend server
└── frontend/
    ├── index.html        # Main HTML file
    ├── package.json      # Frontend dependencies
    ├── tailwind.config.js# Tailwind CSS config
    ├── vite.config.js    # Vite config
    └── ...               # React components and assets
```

---

## Backend Setup
1. Navigate to the backend folder:
   ```sh
   cd backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Configure your MongoDB connection in `config/database.js`.
4. Start the backend server:
   ```sh
   npm start
   ```
   The server will run on the port specified in your configuration (commonly 5000).

---

## Frontend Setup
1. Navigate to the frontend folder:
   ```sh
   cd frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the development server:
   ```sh
   npm run dev
   ```
   The app will be available at `http://localhost:5173` (default Vite port).

---

## API Overview
The backend exposes RESTful APIs for managing events, tickets, sponsors, users, feedback, and user activities. Main route files are in `backend/routes/` and controllers in `backend/controllers/`.

- **/api/events**: Event CRUD operations
- **/api/tickets**: Ticket booking and management
- **/api/sponsors**: Sponsor applications
- **/api/users**: User registration, login, and management
- **/api/feedback**: Event feedback
- **/api/user-activity**: User activity tracking

Refer to the route and controller files for detailed API endpoints and request/response formats.

---

## License
This project is for educational purposes.
