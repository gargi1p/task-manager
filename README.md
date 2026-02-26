# 📌 Task Management System (PHP MVC)

![PHP](https://img.shields.io/badge/PHP-Core-blue)
![MySQL](https://img.shields.io/badge/Database-MySQL-orange)
![Bootstrap](https://img.shields.io/badge/Frontend-Bootstrap%205-purple)
![Architecture](https://img.shields.io/badge/Architecture-MVC-success)

A simple and clean **Task Management System** built using **Core PHP
(MVC Architecture)**, **MySQL**, and **Bootstrap 5**.

------------------------------------------------------------------------

## 📖 Overview

This application allows users to:

-   ✅ Create tasks\
-   📋 View all tasks\
-   ✏️ Update tasks\
-   🗑️ Delete tasks\
-   🔎 Search tasks

Designed using the **MVC (Model-View-Controller)** pattern for better
structure and maintainability.

------------------------------------------------------------------------

## 🏗️ Technology Stack

  Layer             Technology Used
  ----------------- ------------------------
  Backend           Core PHP (MVC Pattern)
  Database          MySQL
  Frontend          HTML, CSS, Bootstrap 5
  Server            Apache (XAMPP)
  Version Control   Git & GitHub

------------------------------------------------------------------------

## 🧠 Architecture -- MVC Pattern

### 🔹 Model

-   Handles database queries\
-   Performs CRUD operations\
-   Contains business logic\
-   Uses secure PDO prepared statements

### 🔹 View

-   Handles UI (HTML + Bootstrap)\
-   Displays forms and tables\
-   Manages user interaction

### 🔹 Controller

-   Handles routing\
-   Connects Model and View\
-   Processes user input

### ✅ Benefits

-   Separation of concerns\
-   Better maintainability\
-   Scalable code structure

------------------------------------------------------------------------

## 🗄️ Database Design

### Database: `task_manager`

### Table: `tasks`

| Column Name | Data Type                | Description                       |
| ----------- | ------------------------ | --------------------------------- |
| id          | INT (PK, AUTO_INCREMENT) | Unique Task ID                    |
| title       | VARCHAR(255)             | Task title                        |
| description | TEXT                     | Task details                      |
| due_date    | DATE                     | Deadline                          |
| status      | VARCHAR(50)              | Pending / In Progress / Completed |
| remarks     | TEXT                     | Additional comments               |
| created_on  | TIMESTAMP                | Record creation time              |
| updated_on  | TIMESTAMP                | Last update time                  |
| created_by  | VARCHAR(100)             | Creator name                      |
| updated_by  | VARCHAR(100)             | Last modifier                     |

------------------------------------------------------------------------

## 🚀 Features

-   Add new task\
-   View tasks in tabular format\
-   Edit task\
-   Delete task\
-   Search by title or status\
-   Secure database operations using PDO\
-   Responsive UI with Bootstrap

------------------------------------------------------------------------

## 📂 Project Structure

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

------------------------------------------------------------------------

## ⚙️ Installation Guide

### 1️⃣ Install XAMPP

Download and install XAMPP.

### 2️⃣ Move Project

Place inside:

    C:\xampp\htdocs\task-manager

### 3️⃣ Create Database

``` sql
CREATE DATABASE task_manager;
```

Then create the `tasks` table using your SQL script.

### 4️⃣ Configure Database

Edit:

    config/database.php

Update credentials if needed.

### 5️⃣ Run Project

Open:

    http://localhost/task-manager

------------------------------------------------------------------------

## 🔐 Security

-   PDO Prepared Statements used\
-   Protection against SQL Injection\
-   No direct SQL string concatenation\
-   Clean MVC separation

------------------------------------------------------------------------

## 📈 Future Improvements

-   User authentication system\
-   Role-based access control\
-   Pagination\
-   Task filtering by date\
-   REST API version\
-   Deployment to live server

------------------------------------------------------------------------

## 🎯 Learning Outcomes

-   MVC Architecture understanding\
-   Database schema design\
-   CRUD implementation\
-   Secure backend coding\
-   Frontend & backend integration\
-   Professional documentation

------------------------------------------------------------------------

## 👩‍💻 Author

**Gargi Singh**\
Aspiring Full Stack Developer

