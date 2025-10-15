# Integrated Hotel Management System (IHMS)

A robust, centralized web-based application designed to automate and streamline core operational processes within a modern hotel. The IHMS enhances efficiency, improves guest satisfaction, and provides management with real-time data for informed decision-making across all departments.

---

## Table of Contents
- [Key Features](#key-features)
- [Application Architecture](#application-architecture)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Setup and Installation](#setup-and-installation)
- [Running the Application](#running-the-application)
- [About the Developers](#about-the-developers)
- [License](#license)

---

## Key Features

- **Front Office Management:** Automated Check-in/Check-out processes, real-time room status updates, and dynamic room assignment.  
- **Centralized Reservations:** Seamless management of direct and channel-based bookings, with detailed availability calendars.  
- **Billing & Folio Management:** Instantaneous invoice generation, support for various payment methods, and automated tax calculations.  
- **Housekeeping Integration:** Real-time room status updates between the front desk and housekeeping staff, minimizing turnaround time.  
- **Inventory Control:** Tracking stock levels for F&B, linen, and general supplies, with low-stock alerts.  
- **Reporting & Analytics:** Generation of KPIs like RevPAR and ADR for management analysis.  

---

## Application Architecture

This project utilizes a **Three-Tier architecture** to ensure scalability and maintainability.

### Frontend (Client-Side)
Built using **React/Angular/HTML & JavaScript**.  
Responsible for user interactions, displaying real-time data, and ensuring a fast, responsive UI/UX.  
Communicates with the Backend API via RESTful endpoints.

### Backend (Server-Side)
Implemented using **Java**.  
Handles business logic, data validation, and security (authentication and authorization).  
Provides necessary API endpoints consumed by the frontend.

### Database (Data-Tier)
Utilizes **MySQL** to securely manage all transactional data, including guest profiles, reservations, room status, and financial records.

---

## Technology Stack

| Component | Technology |
|------------|-------------|
| Core Language | Java |
| Backend Framework | Django |
| ORM/Data Access | SQLAlchemy |
| Authentication | JWT (JSON Web Tokens) |
| Frontend | React |
| Styling/UI | Bootstrap |
| Database | PostgreSQL |

---

## Project Structure

```
hotel-management-system/
├── frontend/              # Client-side code
│   └── src/
├── backend/               # Server-side code
│   └── src/
│   └── config/            # Configurations
├── database/              # SQL schema/migration scripts
│   └── schema.sql
├── requirements.txt       # Dependencies
└── README.md              # Documentation
```

---

## Setup and Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Manu-krishnan005/HotelManagement.git
cd HotelManagement
```

### 2. Create a Virtual Environment

**For Python:**
```bash
python -m venv venv
source venv/bin/activate
```

**For Node.js (if applicable):**
```bash
npm install
```

### 3. Database Configuration
- Install and start your MySQL/PostgreSQL server.
- Create a database named `your_database_name`.
- Load the initial schema:
```bash
psql -U your_user -d your_database_name -f database/schema.sql
```
- Update credentials in `backend/config/application.properties` or `.env`.

### 4. Install Dependencies
**Backend:**
```bash
cd backend
pip install -r requirements.txt
```
**Frontend:**
```bash
cd ../frontend
npm install
```

---

## Running the Application

The application requires two terminal sessions for backend and frontend.

### Start the Backend Server
```bash
cd backend
python manage.py runserver
```
Runs at: [http://localhost:8080](http://localhost:8080)

### Start the Frontend Application
```bash
cd frontend
npm start
```
Runs at: [http://localhost:3000](http://localhost:3000)

### Default Credentials
| Role | Username | Password |
|-------|-----------|-----------|
| Administrator | admin | [secure_password] |
| Front Desk | desk | [secure_password] |

---

## About the Developers

**Naveen Jayaraj**  
3rd Year B.Tech CSE (AIML)  
[LinkedIn](https://www.linkedin.com/in/naveen-jayaraj/)

**Manu Krishnan**  
3rd Year B.Tech CSE (AIML)  
[LinkedIn](https://www.linkedin.com/in/manu-krishnan005)

---

## License

### MIT License

Copyright (c) 2025 Manu Krishnan

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
