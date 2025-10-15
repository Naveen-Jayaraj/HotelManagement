Integrated Hotel Management System (IHMS)
A robust, centralized web-based application designed to automate and streamline core operational processes within a modern hotel. The IHMS enhances efficiency, improves guest satisfaction, and provides management with real-time data for informed decision-making across all departments.

Table of Contents
Key Features

Application Architecture

Technology Stack

Project Structure

Setup and Installation

Running the Application

About the Developers

License

Key Features
Front Office Management: Automated Check-in/Check-out processes, real-time room status updates, and dynamic room assignment.

Centralized Reservations: Seamless management of direct and channel-based bookings, with detailed availability calendars.

Billing & Folio Management: Instantaneous invoice generation, support for various payment methods, and automated tax calculations.

Housekeeping Integration: Real-time room status updates between the front desk and housekeeping staff, minimizing turnaround time.

Inventory Control: Tracking stock levels for F&B, linen, and general supplies, with low-stock alerts.

Reporting & Analytics: Generation of key performance indicators (KPIs) like RevPAR (Revenue Per Available Room) and ADR (Average Daily Rate) for management analysis.

Application Architecture
This project utilizes a Three-Tier architecture to ensure scalability and maintainability.

Frontend (Client-Side)
Built using [e.g., React/Angular/HTML & JavaScript].

Responsible for all user interactions, displaying real-time data, and ensuring a fast, responsive user interface (UI/UX).

Communicates with the Backend API via RESTful endpoints to fetch and submit data.

Backend (Server-Side)
Implemented using Java.

Handles all business logic, data validation, and security (user authentication and authorization).

Manages the connection pool and CRUD operations for the database.

Provides the necessary API endpoints consumed by the frontend.

Database (Data-Tier)
A persistent store utilizing MySQL to securely manage all transactional data, including guest profiles, reservations, room status, and financial records.

Technology Stack
Core Language:
Java

Backend:
Framework: Django

ORM/Data Access: SQLAlchemy

Authentication: JWT (JSON Web Tokens)

Frontend:
Framework: React

Styling/UI: Bootstrap

Database:
Database Management System (DBMS): PostgreSQL

Project Structure
The project is organized into the following file structure:

hotel-management-system/
│
├── frontend/             # All client-side code (HTML, CSS, JS/React/etc.)
│   └── src/
├── backend/              # All server-side code (Business logic, API endpoints)
│   ├── src/
│   └── config/           # Database and security configurations
├── database/             # SQL schema/migration scripts
│   └── schema.sql        # Initial database structure
├── requirements.txt      # Python/Node/Maven dependencies for the project
└── README.md             # This documentation file.
Setup and Installation
To run this project locally, follow these steps.

1. Clone the Repository
Bash

git clone https://github.com/Manu-krishnan005/HotelManagement.git
cd HotelManagement
2. Create a Virtual Environment (Recommended for Python/Node.js)
Bash

# For Python
python -m venv venv
source venv/bin/activate

# For Node.js (if applicable)
# npm install
3. Database Configuration
Install and start your [e.g., MySQL/PostgreSQL] server.

Create a database named [your_database_name].

Load the initial schema:

Bash

psql -U your_user -d your_database_name -f database/schema.sql
Update the database credentials in the backend configuration file located at [backend/config/application.properties] or .env.

4. Install Dependencies
Navigate to the respective folders and install dependencies:

Bash

# Backend Dependencies
cd backend
[e.g., pip install -r requirements.txt or mvn install]

# Frontend Dependencies
cd ../frontend
[e.g., npm install or yarn install]
Running the Application
The application requires two separate terminal sessions to run the backend and frontend simultaneously.

1. Start the Backend Server
Open a terminal, navigate to the backend directory, and run the application:

Bash

cd backend
[e.g., python manage.py runserver or java -jar target/app.jar]
The server should start on http://localhost:[Backend_Port, e.g., 8080].

2. Start the Frontend Application
Open a second terminal, navigate to the frontend directory, and run the development server:

Bash

cd frontend
[e.g., npm start or ng serve]
This will launch the application in your default web browser, accessible at a local URL provided in the terminal (e.g., http://localhost:3000).

Default Credentials (Example)
Role	Username	Password
Administrator	admin	[secure_password]
Front Desk	desk	[secure_password]

Export to Sheets
About the Developers
This project was developed by:

Naveen Jayaraj

3 Year Students Btech CSE AIML

https://www.linkedin.com/in/naveen-jayaraj/

Manu Krishnan

3 Year Students Btech CSE AIML

https://www.linkedin.com/in/manu-krishnan005

License
This project is licensed under the MIT License. See the LICENSE file for details.

Markdown

MIT License

Copyright (c) 2025 Manu Krishnan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
