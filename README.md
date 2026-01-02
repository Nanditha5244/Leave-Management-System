# Leave Management System

This project will be developed step by step as part of my learning process.

Day 1 – Project Setup & Requirement Analysis
✅ Completed Tasks:

Understood project requirements for the Leave Management System

Defined system modules and user roles (Admin, Manager, Employee)

Designed basic application flow and architecture

Set up Spring Boot project using Spring Initializr

Configured project dependencies:

Spring Web

Spring Data JPA

Spring Security

MySQL Driver

Lombok

Configured application.properties for database connection

Verified project build and application startup

Initialized Git repository and pushed initial project structure

🛠️ Technologies Used

Java

Spring Boot

Maven

MySQL

Git & GitHub

Spring Tool Suite (STS)

📌 Output

✔ Project setup completed successfully
✔ Application running without errors
✔ Ready for backend module development

Day 2 – Backend Setup & Authentication Module
✅ Completed Tasks:

Created Spring Boot backend project

Configured project structure using MVC architecture

Implemented User Entity and Role Entity

Created Repository layer using JPA

Implemented Service layer for business logic

Created REST APIs for:

User registration

User login

Implemented JWT-based authentication

Configured Spring Security

Enabled role-based access control

Tested APIs using Postman

🛠️ Technologies Used

Java

Spring Boot

Spring Security

JWT (JSON Web Token)

Hibernate / JPA

MySQL

Maven

📂 Project Structure
src/main/java
 ├── controller
 ├── service
 ├── repository
 ├── entity
 ├── config
 └── security

 🚀 How to Run the Project

Clone the repository

Open in Spring Tool Suite (STS)

Configure database in application.properties

Run the application

Test APIs using Postman
Day 3 – Frontend Implementation (React + Axios)

✅ Completed Tasks:

Set up React frontend for the Leave Management System

Installed required dependencies:

react-router-dom for page routing

axios for API calls

bootstrap & react-icons for styling and UI

Created frontend pages:

Login Page – user login

Register Page – user registration

Apply Leave Page – apply for leave

Leave History Page – view leave history

Admin Dashboard – admin view for all leaves

Implemented React Router for navigation:

/ → Login

/register → Register

/apply → Apply Leave

/history → Leave History

/admin → Admin Dashboard

Integrated axios to call Spring Boot backend APIs:

/auth/register → register user

/auth/login → login user

/leave/apply/{userId} → apply leave

/leave/user/{userId} → view user leave history

/leave/all → admin view all leaves

/leave/status/{leaveId} → update leave status

Added Bootstrap styling for forms, buttons, and navbar

Added react-icons for better UI/UX

Configured CORS in backend to allow frontend (http://localhost:3000) communication

Tested frontend-backend integration successfully:

User can register → login → apply leave → view history

Admin can view and update leave requests

🛠️ Technologies Used:

React.js

Axios

React Router DOM

Bootstrap

React Icons

JavaScript

HTML & CSS

📂 Project Structure

src
 ├── App.js
 ├── index.js
 ├── pages
 │    ├── Login.js
 │    ├── Register.js
 │    ├── ApplyLeave.js
 │    ├── LeaveHistory.js
 │    └── AdminDashboard.js
 └── components
      └── Navbar.js


🚀 How to Run the Frontend

Navigate to frontend project folder in terminal

Run npm install to install dependencies

Run npm start to start the development server

Open http://localhost:3000 in the browser

Register a new user → login → apply leaves → view history → access admin dashboard

📌 Output

✔ Frontend running successfully
✔ User can register, login, apply leave, and view leave history
✔ Admin can view all leaves and update status
✔ Integrated and tested with backend APIs