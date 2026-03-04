<div align="center">

# 💖✨ HMS Pro ✨💖  
### 🌸 A Beautiful & Elegant Hostel Management System 🌸  

<i>Smart. Simple. Stylish. Built with care & a little bit of magic. 🪄</i>  

<br>

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
<img src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" />
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />

<br><br>

💌 <i>Made with dedication, coffee, and a little extra love.</i>

</div>

---

# 🎀 Table of Contents

- 🌷 [About HMS Pro](#-about-hms-pro)
- 📁 [Project Structure](#-project-structure)
- 🚀 [Getting Started](#-getting-started)
- 💻 [How To Use](#-how-to-use)
- ✨ [Features](#-features)
- 🔐 [Security Notes](#-security-notes)
- 🌸 [Final Words](#-final-words)

---

# 🌷 About HMS Pro

**HMS Pro** is a web-based Hostel Management System designed to make hostel administration smooth, beautiful, and stress-free.

It helps manage:

- 👩‍🎓 Students  
- 🛏 Rooms  
- 🏢 Hostels  
- 📅 Attendance  
- 💰 Fees  
- 👤 Users (Admins & Wardens)

Built using:

- 🐍 Python (Flask)
- 🐬 MySQL
- 🌐 HTML, CSS, JavaScript

This system combines **clean backend logic** with a **soft, elegant frontend UI** — powerful on the inside, pretty on the outside 💕

---

# 📁 Project Structure

Here’s how everything is organized:


HMS-Pro/
│
├── app.py
├── schema.sql
├── index.html
├── login.html
│
└── assets/
├── css/
│ └── style.css
└── js/
└── app.js


---

## ⚙️ Backend (The Engine 💗)

### 🌸 `app.py`
The main Flask application.

**Responsibilities:**
- Routing (`/login`, `/dashboard`, `/api/...`)
- Session management
- Authentication
- Database communication
- REST-style API endpoints

It connects the frontend with the MySQL database and ensures everything runs smoothly.

---

### 🌸 `schema.sql`
The database blueprint.

It creates the database:


hostel_db


And tables:

- `users`
- `hostels`
- `rooms`
- `students`
- `attendance`
- `fees`

It also includes sample data so you can start instantly.

---

## 🖥️ Frontend (The Beauty ✨)

### 🌸 `login.html`
The secure gateway.

- Elegant login form
- Clean UI
- Safe authentication

---

### 🌸 `index.html`
The main dashboard.

Contains:
- Statistics cards
- Navigation sidebar
- Sections for:
  - Students
  - Rooms
  - Attendance
  - Fees
  - Users

Everything loads dynamically using JavaScript — no full page reloads.

---

## 🎨 Assets (The Style & Brain 🧠✨)

### 🌸 `assets/css/style.css`
The aesthetic heart of the project.

- Gradient backgrounds
- Glassmorphism UI
- Smooth transitions
- Modern layout
- Responsive design

---

### 🌸 `assets/js/app.js`
The interactive logic.

Handles:
- Fetching data using `fetch()`
- Updating dashboard dynamically
- Handling user actions
- API communication

---

# 🚀 Getting Started

Let’s set it up on your machine 🌷

---

## 🛠 Prerequisites

Make sure you have:

- Python 3.x
- MySQL Server
- pip

---

## 1️⃣ Install Dependencies

```bash
pip install Flask flask-mysqldb
2️⃣ Setup Database

Make sure MySQL is running.

Run:

cmd.exe /c "mysql -u root -p < schema.sql"

Enter your MySQL password when prompted.

3️⃣ Configure Database

Open app.py and update:

app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'root'
app.config['MYSQL_PASSWORD'] = 'admin'  # Change if needed
app.config['MYSQL_DB'] = 'hostel_db'
4️⃣ Run The App
python app.py

Open:

http://127.0.0.1:5000

And enjoy 🌸

💻 How To Use
🔑 Login

Default accounts:

Admin:

Username: Admin
Password: root

Warden:

Username: warden
Password: warden123
📊 Dashboard

See:

Total Students

Room Availability

Attendance Stats

Pending Fees

👩‍🎓 Students

Add new students

Assign rooms

View details

Manage records

🛏 Rooms

Track capacity

Monitor occupancy

See available rooms

📅 Attendance

Mark daily presence

Review records

💰 Fees

Track paid amounts

Monitor pending dues

👤 Users (Admin Only)

Add new wardens

Manage access control

✨ Features

🌸 Role-based authentication
🌸 Dynamic dashboard analytics
🌸 Real-time data fetching
🌸 Clean REST-style API
🌸 Responsive UI
🌸 Beautiful modern design
🌸 Organized database structure

🔐 Security Notes

⚠️ Current version:

Passwords stored in plain text

Secret key hardcoded

Debug mode enabled

For production:

Use password hashing (werkzeug.security)

Use environment variables

Disable debug mode

Add validation & error handling

🌸 Final Words

HMS Pro is more than just a project —
it’s a blend of logic and elegance.

Built with:

💡 Intelligence

🎨 Creativity

💖 Dedication

And maybe… just a little extra love for someone special.

<div align="center">
💕 Made with care, crafted with passion, and designed to impress 💕
</div> ```