📌 Task Management System (PHP MVC)








A simple and clean Task Management System built using Core PHP (MVC Architecture), MySQL, and Bootstrap 5.

This project demonstrates strong fundamentals of backend development, database design, and MVC architecture.

📖 Overview

This application allows users to:

✅ Create tasks

📋 View all tasks

✏️ Update tasks

🗑️ Delete tasks

🔎 Search tasks

It is designed following the MVC (Model-View-Controller) pattern to ensure clean structure and maintainability.

🏗️ Technology Stack
Layer	Technology Used
Backend	Core PHP (MVC Pattern)
Database	MySQL
Frontend	HTML, CSS, Bootstrap 5
Server	Apache (XAMPP)
Version Control	Git & GitHub
🧠 Architecture Used – MVC Pattern

This project follows the Model-View-Controller (MVC) architecture.

🔹 Model

Responsible for:

Database queries

CRUD operations

Business logic

Secure PDO operations

🔹 View

Responsible for:

UI (HTML + Bootstrap)

Forms & tables

User interaction

🔹 Controller

Responsible for:

Routing requests

Connecting Model and View

Processing user input

✅ Benefits of MVC

Separation of concerns

Better code organization

Easy maintenance

Scalable structure

🗄️ Database Design
📌 Database Name:
task_manager
📌 Table: tasks
Column Name	Data Type	Description
id	INT (PK, AUTO_INCREMENT)	Unique Task ID
title	VARCHAR(255)	Task title
description	TEXT	Task details
due_date	DATE	Deadline
status	VARCHAR(50)	Pending / In Progress / Completed
remarks	TEXT	Additional comments
created_on	TIMESTAMP	Record creation time
updated_on	TIMESTAMP	Last update time
created_by	VARCHAR(100)	Creator name
updated_by	VARCHAR(100)	Last modifier
🔎 Indexing

id is Primary Key (Automatically Indexed)

Improves search and retrieval performance

🧩 Conceptual ER Structure
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
🛠️ Development Approach
📌 Database-First Approach

Database schema designed first

PHP models built based on existing schema

Suitable for small to medium-scale applications

🚀 Features Implemented

➕ Add new task

📋 View tasks in tabular format

✏️ Edit task

🗑️ Delete task

🔎 Search by title or status

🔐 Secure database operations using PDO

📱 Responsive UI with Bootstrap 5

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

C:\xampp\htdocs\task-manager
Step 3: Create Database

Open phpMyAdmin and run:

CREATE DATABASE task_manager;

Then create the tasks table using your SQL script.

Step 4: Configure Database

Open:

config/database.php

Update credentials if needed:

host: localhost
username: root
password: ""
database: task_manager
Step 5: Run Project

Open your browser and go to:

http://localhost/task-manager
🔐 Security Considerations

✅ PDO Prepared Statements used

✅ Prevents SQL Injection

✅ No direct SQL concatenation

✅ MVC separation improves structure & safety

📈 Possible Future Improvements

🔑 User authentication system

👥 Role-based access control

📄 Pagination

📅 Task filtering by date

🌐 REST API version

🚀 Deployment to live server

🎯 Learning Outcomes

This project demonstrates:

✔️ Understanding of MVC architecture

✔️ Database schema design

✔️ CRUD implementation

✔️ Secure backend coding using PDO

✔️ Frontend integration with backend

✔️ Professional project documentation
