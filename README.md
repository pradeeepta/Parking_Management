# Parking Management System

A comprehensive web application for managing parking facilities, built using **Spring Boot** and **React**.

## 🚀 Overview

The Parking Management System streamlines the process of managing and booking parking slots. It provides an intuitive user interface for customers and a robust dashboard for administrators to efficiently manage the facility.

## ✨ Features

### 👤 User Features
- User registration and login with JWT-based authentication
- View available parking slots
- Book parking slots
- Manage existing bookings
- User dashboard with booking history

### 🛠️ Admin Features
- Admin dashboard with system overview
- Manage parking slots (add, update, delete)
- View and manage all bookings
- Manage user accounts
- Configure system settings

## 🛠 Technology Stack

### Backend
- Java 21
- Spring Boot 3.2.2
- Spring Security with JWT Authentication
- Spring Data MongoDB
- Maven for dependency management

### Frontend
- React 18
- React Router for navigation
- Material-UI for responsive design
- Axios for API communication

### Database
- MongoDB

## ⚙️ Setup & Installation

### Prerequisites
- Java 21+
- Node.js and npm
- MongoDB running locally or remotely

### Backend Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/pradeeepta/Parking_Management.git
   ```
2. Navigate to the backend directory (if separate).
3. Build the project:
   ```bash
   mvn clean install
   ```
4. Start the backend server:
   ```bash
   mvn spring-boot:run
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install frontend dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```

## 🗄 Database Configuration

Make sure MongoDB is running and accessible. You can configure the connection in the `application.properties` file (usually located under `src/main/resources` in the backend):

```properties
spring.data.mongodb.host=localhost
spring.data.mongodb.port=27017
spring.data.mongodb.database=parking_management
```

## 🧪 Usage

### User Access
- Register a new user account
- Login with your credentials
- View available parking slots
- Book a slot for a specific time period
- View and manage your bookings via the dashboard

### Admin Access
- Login with admin credentials
- Access the admin dashboard
- Manage parking slots, users, and bookings
- Configure system-wide settings

## 📁 Project Structure

### Backend
```
├── controller         # REST API controllers
├── model              # Data models (entities)
├── repository         # MongoDB repositories
├── service            # Business logic
├── security           # JWT and security configuration
├── dto                # Data Transfer Objects
└── util               # Utility classes
```

### Frontend
```
├── components         # Reusable UI components
├── contexts           # React contexts for state management
├── pages              # User-facing pages
└── pages/admin        # Admin-specific views
```

