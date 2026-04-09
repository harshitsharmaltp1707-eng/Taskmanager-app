# Taskmanager-app
Task Management System built with Laravel, featuring authentication, role-based access (Admin/User), task CRUD, file uploads, filtering, and dashboard summary.
# Task Management System (Laravel + React)

A modern Task Management System built using Laravel (backend) and React (frontend). This project demonstrates authentication, role-based access control, and full CRUD operations with file upload and filtering features.

---

##  Tech Stack

### Backend

* Laravel
* PHP 8.x
* MySQL (XAMPP)

### Frontend

* React.js
* Vite
* Axios

---

##  Features

###  Authentication

* User Registration & Login
* Protected routes (only logged-in users)

### 🧑‍🤝‍🧑 User Roles

* **Admin**

  * View all tasks
  * Delete any task
* **User**

  * Create tasks
  * Manage only their own tasks

### 📋 Task Management

* Create, Read, Update, Delete tasks
* Fields:

  * Title (required)
  * Description
  * Priority (Low / Medium / High)
  * Deadline
  * Status (Pending / Completed)

### 📎 File Upload

* Attach one file per task
* Supported formats: PDF, JPG, PNG
* Max size: 2MB

### 🔍 Filtering

* Filter tasks by:

  * Status
  * Priority

### 📊 Dashboard

* Total tasks
* Completed tasks
* Pending tasks
* Role-based view

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Taskmanager-app.git
cd Taskmanager-app
```

### 2. Install dependencies

```bash
composer install
npm install
```

### 3. Setup environment

```bash
cp .env.example .env
php artisan key:generate
```

### 4. Configure database in `.env`

```env
DB_DATABASE=task_manager
DB_USERNAME=root
DB_PASSWORD=
```

### 5. Run migrations

```bash
php artisan migrate
```

### 6. Run development servers

```bash
npm run dev
php artisan serve
```

---

##  Application URLs

* Backend: http://127.0.0.1:8000
* Frontend (Vite): http://localhost:5173

---

##  Admin Access

To make a user admin:

1. Open phpMyAdmin
2. Go to `users` table
3. Set:

```
role = admin
```

---

##  Project Structure

* `app/` → Backend logic (Laravel)
* `resources/js/` → React frontend
* `routes/web.php` → Routes
* `database/` → Migrations

---

##  Security

* `.env` is not included
* Use `.env.example` for setup

---

* Dashboard
* Task List
* Create Task Page

---

##  Conclusion

This project demonstrates a full-stack application using Laravel and React, including authentication, role-based authorization, and CRUD operations — making it ideal for portfolio and learning purposes.

---

##  Author

**Harshit Sharma**
