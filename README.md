Employee Management System

 PHP & MySQL CRUD Application
A clean and professional **Employee Management System** built using
**PHP, MySQL, and Bootstrap 5**.\
This web application demonstrates full **CRUD (Create, Read, Update,
Delete)** operations with database integration.

------------------------------------------------------------------------

##  Project Overview

This project allows users to:

-   Add new employees\
-   View employee records\
-   Update employee details\
-   Delete employee records

It is designed as a backend-focused CRUD system suitable for academic
and learning purposes.

------------------------------------------------------------------------

Features

### 🔹 Core Functionality

Create new employee records\
Read & display employees in a structured table\
Update employee information\
Delete employees from database

### 🔹 User Interface

Responsive Bootstrap 5 layout\
Clean table design\
HTML5 form validation\
Simple navigation flow

------------------------------------------------------------------------

 Database Schema

### Database Name:

`employee_db`

### Table: `employees`

  Column       Type            Description
  ------------ --------------- ----------------------
  id           INT (PK, AI)    Unique employee ID
  name         VARCHAR(100)    Employee full name
  email        VARCHAR(100)    Employee email
  position     VARCHAR(100)    Job title
  salary       DECIMAL(10,2)   Employee salary
  created_at   TIMESTAMP       Record creation time

### SQL Table Creation Script

``` sql
CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL,
    position VARCHAR(100) NOT NULL,
    salary DECIMAL(10,2) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

------------------------------------------------------------------------

#Installation & Setup

###  Requirements

-   Laragon / XAMPP / WAMP
-   PHP 7.4 or higher
-   MySQL 5.7 or higher
-   Web Browser

------------------------------------------------------------------------

###  Setup Instructions

1️⃣ Clone the repository or download ZIP.

2️⃣ Place project folder inside:

`C:\laragon\www\`

3️⃣ Create database named:

`employee_db`

4️⃣ Run the SQL table creation script above.

5️⃣ Open browser and navigate to:

`http://localhost/employee-crud/`

------------------------------------------------------------------------

##  Project Structure

    employee-crud/
    ├── config.php
    ├── index.php
    ├── create.php
    ├── edit.php
    ├── delete.php
    ├── style.css
    └── README.md

------------------------------------------------------------------------

##  CRUD Operations

  Operation   SQL Query
  ----------- -----------------------------------
  Create      INSERT INTO employees
  Read        SELECT \* FROM employees
  Update      UPDATE employees SET ... WHERE id
  Delete      DELETE FROM employees WHERE id
