.

📌 Task Management System (PHP MVC)
📖 Overview

This project is a Task Management System developed using Core PHP (MVC Architecture), MySQL, and Bootstrap 5.

The application allows users to:

Create tasks

View all tasks

Update tasks

Delete tasks

Search tasks

The project demonstrates understanding of:

MVC Architecture

Database design

CRUD operations

Search functionality

Secure database handling using PDO

Clean UI using Bootstrap

🏗️ Technology Stack
Layer	Technology Used
Backend	Core PHP (MVC Pattern)
Database	MySQL
Frontend	HTML, CSS, Bootstrap 5
Server	Apache (XAMPP)
Version Control	GitHub
🧠 Architecture Used

This project follows the MVC (Model-View-Controller) pattern.

Model

Handles:

Database queries

Data operations (CRUD)

Business logic

View

Handles:

UI (HTML + Bootstrap)

Forms and tables

User interaction

Controller

Handles:

Routing

Connecting Model and View

Processing user input

This structure ensures:

Separation of concerns

Better maintainability

Scalable code design

🗄️ Database Design
Database Name:
task_manager
Table: tasks
Column Name	Data Type	Description
id	INT (PK, AUTO_INCREMENT)	Unique Task ID
title	VARCHAR(255)	Task title
description	TEXT	Task details
due_date	DATE	Deadline
status	VARCHAR(50)	Task status (Pending / In Progress / Completed)
remarks	TEXT	Additional comments
created_on	TIMESTAMP	Record creation time
updated_on	TIMESTAMP	Last update time
created_by	VARCHAR(100)	Creator name
updated_by	VARCHAR(100)	Last modifier
ER Diagram (Conceptual)
Task
-------------------------------------
id (PK)
title
description
due_date
status
remarks
created_on
updated_on
created_by
updated_by
Indexing

id is Primary Key (Automatically Indexed)

Improves search and retrieval performance

Approach Used

This project uses:

Database First Approach

Reason:

Database structure was designed first.

PHP models were built based on existing schema.

Suitable for small-to-medium applications.

🚀 Features Implemented

Add new task

View all tasks in tabular format

Edit task

Delete task

Search task by title or status

Secure database operations using PDO prepared statements

Responsive UI using Bootstrap

📂 Project Structure
task-manager/
│
├── config/
│   └── database.php
│
├── models/
│   └── Task.php
│
├── controllers/
│   └── TaskController.php
│
├── views/
│   ├── header.php
│   ├── footer.php
│   ├── task_list.php
│   ├── create_task.php
│   ├── edit_task.php
│
├── index.php
└── README.md
⚙️ Installation & Setup Guide
Step 1: Install XAMPP

Download and install XAMPP.

Step 2: Move Project

Place the project folder inside:

htdocs/

Example:

C:\xampp\htdocs\task-manager
Step 3: Create Database

Open phpMyAdmin and run:

CREATE DATABASE task_manager;

Then create tasks table using provided SQL script.

Step 4: Configure Database

Open:

config/database.php

Update credentials if needed:

host: localhost
username: root
password: ""
database: task_manager
Step 5: Run Project

Open browser and go to:

http://localhost/task-manager
🔐 Security Considerations

PDO Prepared Statements used to prevent SQL Injection

No direct SQL string concatenation

Basic MVC separation improves maintainability

📈 Possible Improvements

User authentication system

Role-based access control

Pagination

Task filtering by date

API version of application

Deployment to live server

🎯 Learning Outcomes

This project demonstrates:

Understanding of MVC architecture

Database schema design

CRUD implementation

Secure backend coding

Frontend integration with backend

Project documentation skills

