<div align="center">

# 💖✨ HMS Pro ✨💖  
### 🌸 Modern Hostel Management System Built with Flask 🌸  

<img src="https://img.shields.io/github/license/yourusername/hms-pro?style=for-the-badge" />
<img src="https://img.shields.io/github/stars/yourusername/hms-pro?style=for-the-badge" />
<img src="https://img.shields.io/github/forks/yourusername/hms-pro?style=for-the-badge" />
<img src="https://img.shields.io/github/issues/yourusername/hms-pro?style=for-the-badge" />

<br>

<img src="https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python" />
<img src="https://img.shields.io/badge/Flask-Web_Framework-black?style=flat-square&logo=flask" />
<img src="https://img.shields.io/badge/MySQL-Database-005C84?style=flat-square&logo=mysql" />
<img src="https://img.shields.io/badge/Status-Active-success?style=flat-square" />

<br><br>

### 🚀 Smart. Scalable. Elegant.
A full-featured Hostel Management System with modern UI, dynamic dashboard, and role-based access control.

<br>

⭐ If you like this project, consider giving it a star!

</div>

---

# 📌 Overview

**HMS Pro** is a full-stack web application designed to simplify hostel administration.

It provides a clean dashboard interface for managing:

- 👩‍🎓 Students  
- 🛏 Rooms  
- 🏢 Hostels  
- 📅 Attendance  
- 💰 Fees  
- 👤 Admin & Warden Roles  

Built using:

- Python (Flask)
- MySQL
- HTML5, CSS3
- Vanilla JavaScript (Fetch API)

---

# 🖼 Preview

> *(Add screenshots here for maximum impact)*

```markdown
![Dashboard Screenshot](screenshots/dashboard.png)
![Login Screenshot](screenshots/login.png)

Creating a screenshots/ folder will make this look very professional.

✨ Key Features
🔐 Authentication System

Role-based access (Admin / Warden)

Secure session handling

Login & logout system

📊 Interactive Dashboard

Real-time statistics

Dynamic data loading

Clean analytics cards

👩‍🎓 Student Management

Add & manage students

Assign rooms

View complete records

🛏 Room Allocation

Track occupancy

Capacity monitoring

Available room detection

📅 Attendance Tracking

Daily attendance marking

Attendance history

💰 Fee Management

Paid vs Pending tracking

Simple financial overview

🧱 Project Architecture
Frontend (HTML, CSS, JS)
        ↓
Flask Backend (app.py)
        ↓
MySQL Database (schema.sql)
Backend Responsibilities

Routing

API endpoints

Session management

Database queries

Frontend Responsibilities

UI rendering

Fetch API requests

Dynamic updates

User interactions

📂 Project Structure
HMS-Pro/
│
├── app.py
├── schema.sql
├── index.html
├── login.html
│
└── assets/
    ├── css/
    │   └── style.css
    └── js/
        └── app.js
🚀 Getting Started
1️⃣ Clone the Repository
git clone https://github.com/yourusername/hms-pro.git
cd hms-pro
2️⃣ Install Dependencies
pip install Flask flask-mysqldb
3️⃣ Setup Database

Make sure MySQL is running:

cmd.exe /c "mysql -u root -p < schema.sql"
4️⃣ Configure Database

Edit app.py:

app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'root'
app.config['MYSQL_PASSWORD'] = 'your_password'
app.config['MYSQL_DB'] = 'hostel_db'
5️⃣ Run the App
python app.py

Visit:

http://127.0.0.1:5000
🔮 Roadmap

 Password hashing

 Search & filtering

 Pagination

 Export data (CSV/PDF)

 REST API documentation

 Docker support

 Deployment guide (Render / AWS)

🛡 Security Improvements (Recommended)

Implement password hashing (werkzeug.security)

Store secrets in environment variables

Disable debug mode in production

Add input validation

Use HTTPS when deployed

🤝 Contributing

Contributions are welcome!

Fork the repo

Create your feature branch

Commit changes

Push to your branch

Open a Pull Request

📜 License

This project is licensed under the MIT License.

<div align="center">
💕 Built with passion, logic, and a touch of elegance

If this project helped you, don’t forget to ⭐ star the repository!

</div> ```