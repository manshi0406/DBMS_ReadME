<div align="center">
  <h1>✨ HMS Pro ✨</h1>
  <p><i>A beautiful, elegant, and efficient Hostel Management System</i> 🌸</p>

  <!-- Badges -->
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask" />
  <img src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />

</div>

---

## 🎀 Table of Contents
- [About The Project](#-about-the-project)
- [What's Inside? (Project Structure)](#-whats-inside-project-structure)
- [Getting Started](#️-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation Steps](#installation-steps)
- [How to Use HMS Pro](#-how-to-use-hms-pro)
- [Features](#-features)

---

## 🎀 About The Project

Welcome to **HMS Pro**! This project is a carefully crafted web-based application designed to make managing a hostel an absolute breeze. With a clean interface and robust backend, it handles everything from student records and room assignments to daily attendance and fee tracking. 

Built with love using Python (Flask) and MySQL, it features a comprehensive dashboard for both Administrators and Wardens. 🌷

---

## 📁 What's Inside? (Project Structure)

Every file in this project plays a special role in bringing the application to life. Here's a quick guide to help you find your way around:

### ⚙️ Backend (The Engine)
- 🌸 **`app.py`**  
  *The Heart:* This is the core Flask application. It manages routing, backend logic, and provides the API endpoints (e.g., `/api/login`, `/api/students`). It's responsible for keeping the sessions secure and talking to the database.

- 🌸 **`schema.sql`**  
  *The Data Blueprint:* Contains all the necessary SQL commands to build the `hostel_db` database. It sets up tables for `users`, `hostels`, `rooms`, `students`, `attendance`, and `fees`, complete with some magical mock data to get you started immediately!

### 🖥️ Frontend (The Looks)
- 🌸 **`index.html`**  
  *The Command Center:* The main dashboard interface! It's where admins and wardens view statistics, manage student data, track attendance, and monitor fee statuses in a beautifully organized layout.

- 🌸 **`login.html`**  
  *The Gateway:* A secure and stylish authentication page where users enter their credentials to access the system safely.

### � Assets (The Style)
- � **`assets/css/style.css`**  
  *The Aesthetic:* The stylesheet that brings the design to life. It ensures the layout is gorgeous, modern, and user-friendly.

- 🌸 **`assets/js/app.js`**  
  *The Brain:* The interactive part of the frontend. It fetches data dynamically and handles user actions smoothly without reloading the page.

---

## 🛠️ Getting Started

Ready to run HMS Pro on your own machine? Let's get it set up! 🚀

### Prerequisites
Make sure you have these installed on your computer:
- 🐍 **Python 3.x**
- 🐬 **MySQL Server**
- 📦 **pip** (Python package manager)

### Installation Steps

#### 1. Install the Magic Dependencies
Open your terminal and install the required Python packages:
```bash
pip install Flask flask-mysqldb
```

#### 2. Set Up the Database 🗄️
Let's create the database by running the schema script (make sure your MySQL is running!). If you are using Windows PowerShell, run:
```powershell
cmd.exe /c "mysql -u root -p < schema.sql"
```
*(Enter your MySQL password when prompted!)*

#### 3. Configure the Secrets 🤫
Open `app.py` and find the database configuration section (around line `9`). Update the credentials if your local setup is different:
```python
app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'root'
app.config['MYSQL_PASSWORD'] = 'admin' # ✨ Update this to your MySQL password! ✨
app.config['MYSQL_DB'] = 'hostel_db'
```

#### 4. Launch the App! 🎉
Run the Flask application:
```bash
python app.py
```
The server will bloom at **`http://127.0.0.1:5000`** 🌺

---

## 👩‍💻 How to Use HMS Pro

1. **Log In** 🔑
   - Visit `http://127.0.0.1:5000`
   - Use the default Admin account (*Username: `Admin` | Password: `root`*) or Warden account (*Username: `warden` | Password: `warden123`*).
2. **Explore the Dashboard** 📊
   - Keep track of total students, room availability, today's attendance, and pending fees right at the top!
3. **Manage With Ease** ✨
   - **Students**: Add new residents and assign them a comfy room.
   - **Attendance**: Mark daily attendance quickly.
   - **Fees**: Keep track of who has paid and who is pending.
   - **Users (Admin Only)**: Give access to new wardens to help you out!

---

## ✨ Features

- **Dashboard Analytics**: Quick overview of hostel statistics.
- **Role-based Authentication**: Secure access for Admins and Wardens.
- **Student Management**: Add, view, and organize resident data.
- **Room Allocation**: Track occupancy and unassigned rooms.
- **Attendance Tracking**: Easily mark and review daily presence.
- **Fee Management**: Keep an eye on paid amounts and pending dues.

<br>

<div align="center">
  <i>Created with 💖 and a touch of magic!</i>
</div>
