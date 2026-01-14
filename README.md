# Leave Management System – Backend (Day-wise Implementation)

This document explains the backend development of the Leave Management System
in a clear day-by-day manner. The backend is
This helps in understanding how the system was built step by step.

---

## Day 1 – Project Setup & Database Configuration

On the first day, the backend project was created using Spring Boot.
Basic configurations were done to connect the application with the database.

Key work:
- Created Spring Boot project
- Configured database connection
- Verified application startup
- Created basic project structure

Outcome:
The backend application was successfully connected to the database.

---

## Day 2 – User Registration & Authentication

On the second day, user authentication functionality was implemented.
This allows users to register and log in securely.

Key work:
- User registration logic
- Login validation
- Password encryption
- Token-based authentication

Outcome:
Users can securely register and log in to the system.

---

## Day 3 – Leave Application Module

On the third day, the leave application functionality was developed.
Users can apply for leave by providing required details.

Key work:
- Leave apply API
- Accept start date, end date, and leave type
- Automatic calculation of leave days
- Store leave request with pending status

Outcome:
Users can successfully apply for leave and view submitted requests.

---

## Day 4 – Leave Approval & Rejection

On the fourth day, leave approval and rejection logic was implemented.
Authorized users can take action on pending leave requests.

Key work:
- Approve leave functionality
- Reject leave functionality
- Update leave status in database
- Validate access before approval

Outcome:
Leave requests can be approved or rejected properly.

---

## Day 5 – Leave Balance Calculation

On the fifth day, leave balance functionality was added.
The system automatically calculates used and remaining leaves.

Key work:
- Count approved leaves
- Calculate total used leave days
- Provide remaining leave balance
- Display balance through API

Outcome:
Leave balance updates automatically based on approved leaves.

---

## Day 6 – Security & Validation

On the sixth day, security and validation were strengthened to protect APIs.

Key work:
- API access protection
- Token validation
- Input validation
- Error handling

Outcome:
The backend is secure and prevents unauthorized access.

---

## Day 7 – Testing & Finalization

On the final day, complete backend testing and refinement were done.

Key work:
- API testing using Postman
- Verified leave flow end-to-end
- Fixed errors and edge cases
- Prepared backend for frontend integration

Outcome:
Backend is stable, tested, and ready for frontend usage.

---

## Technologies Used

- Java
- Spring Boot
- Spring Security
- JPA / Hibernate
- MySQL
- Maven

---

## Final Status

The backend of the Leave Management System is fully implemented,
tested, and ready for integration with the frontend.
# LMS Login & OTP Registration Flow

This module implements authentication and onboarding for LMS (Leave Management System) with Admin-controlled OTP registration for Employees & Managers.

---

## 🚀 Features

### 🔐 **Login System**
- Admin, Manager and Employee can login
- Role-based routing:
  | Role | Redirect |
  |------|----------|
  | ADMIN | `/admin-dashboard` |
  | MANAGER | `/manager-dashboard` |
  | EMPLOYEE | `/employee-dashboard` |

- Admin credentials are seeded in database
- Invalid login shows error message

---

### 👥 **Admin-Controlled Registration**
Employee and Manager accounts cannot self-register.

Only Admin can create new accounts from:
