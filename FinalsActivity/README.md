# My Diary Web App

A secure personal diary web application built with **PHP** and **MariaDB**.  
Users can register, log in using a username, manage their profiles, upload gallery images, and write diary entries.  
An **admin panel** allows administrators to manage users and control maintenance mode.

---

## Features

### User
- User registration and login (username-based)
- Password hashing (`password_hash`, `password_verify`)
- Profile with profile picture
- Personal diary entries (create, view, delete)
- Image gallery (upload & delete)
- Session-based authentication

### Admin
- Admin-only panel
- Activate / suspend users
- Maintenance mode control
- Role-based access (`user`, `admin`)
- Tailwind CSS–styled admin interface

---

## Security

- Prepared statements (PDO) to prevent **SQL Injection**
- Output escaping using `htmlspecialchars` to prevent **XSS**
- Password hashing using PHP’s built-in hashing functions
- Session validation for protected pages
- Role-based access control for admin routes

---

## Technologies Used

- **Backend:** PHP (PDO)
- **Database:** MariaDB / MySQL
- **Frontend:**
  - Custom CSS (`style.css`) for user pages
  - Tailwind CSS (CDN) for admin panel
- **Server:** XAMPP (Apache + MariaDB)

---

## Frontend / Styling

- **Admin Panel:** Tailwind CSS (via CDN)
- **User Pages:** Custom CSS (`style.css`)

Example Tailwind inclusion (admin panel only):

```html
<script src="https://cdn.tailwindcss.com"></script>
