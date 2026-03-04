<div align="center">

# 🌸✨ HMS Pro: Hostel Management System ✨🌸

Welcome to the cutest, most organized **Hostel Management System**! 🎀 This project is designed to make managing dormitory life a breeze—from tracking students to managing fees and attendance, all wrapped up in a clean and beautiful interface! 🍰💖

</div>

---

## 🧸 What's Inside? (Features)

This application is packed with adorable and powerful features! 🌷

*   🎀 **Secure Login & Authentication:** Safe access for Admins and Wardens!
  
*   📊 **Sparkling Dashboard:** Get quick stats on students, available rooms, attendance, and pending fees at a single glance! ✨
  
*   👩‍🎓 **Student Management:** Keep track of all the lovely residents, their courses, and guardian info.

*   🚪 **Room Allocation:** Manage singles, doubles, and triples effortlessly.

*   📅 **Attendance Tracking:** Mark who is present, absent, or out having fun! ☁️

*   💰 **Fee Management:** A clean overview of total and pending fees for every student.

*   👑 **Role-Based Access:** Special admin-only areas to manage users!


---

## 💻✨ Built With (Tech Stack)

The magic behind the scenes! 🪄
*   **Backend:** Python 🐍 + Flask 🌶️
*   **Database:** MySQL 🐬 (using `flask_mysqldb`)
*   **Frontend:** HTML, CSS, JavaScript 🎨 (served via Flask templates)

---

## 📂 File Structure (How it Works)

Here is the clean and creative layout of our project files! 🍓

```text
root_dictonary/
│
├── 🌸 app.py           # The heartbeat of the app! Contains all Flask routes and API endpoints.
├── 🌸 schema.sql       # The blueprint! Sets up our shiny database and initial mock data.
├── 🌸 index.html       # The main dashboard view (where the magic happens).
├── 🌸 login.html       # The beautiful entry point for users to log in.
│
└── 🎀 assets/          # Holds all the pretty styling and scripts!
    ├── css/            # Custom stylesheets for that perfect look.
    └── js/             # JavaScript files for interactive sparkles.
```

---

## 🗄️ Database Structure (Our Tables)

A peek into how we store our precious data (`hostel_db`)! 🦋

| Table Name | Description 🎀 |
| :--- | :--- |
| **`users`** | Stores `admin` and `warden` credentials securely. |
| **`hostels`** | Basic info about the hostel building itself. |
| **`rooms`** | Details about room numbers, types, blocks, and occupancy limits. |
| **`students`** | Everything about the students, linked to their assigned `room_id`. |
| **`attendance`** | Daily tracking linked by `student_id` and `date`. |
| **`fees`** | Financial records showing `total_fee`, `paid_amount`, and `status`. |

*(All tables are cleanly linked with foreign keys to ensure data integrity!)* ✨

---

## 🚀 How to Setup & Run!

Ready to get this cute app up and running? Follow these simple steps! 🍰


### Note:
**In My Opinion Run All The Commands In VScode Terminal OR Antigravity Terminal**


### 1️⃣ Database Setup 🐬
1. Make sure you have **MySQL** installed and running on your machine.
2. Open your MySQL command line or client (like phpMyAdmin) and run the magical `schema.sql` script. You can run this command in your terminal:
   ```bash
   cmd.exe /c "mysql -u root -p < schema.sql"
   ```
   *(This creates the `hostel_db` database, its shiny tables, and populates it with some cute mock data!)*

### 2️⃣ Project Requirements 📦
You'll need Python installed! Open your terminal in the `root_dictonary/` directory and install the necessary Flask packages:
```bash
pip install Flask Flask-MySQLdb
```

### 3️⃣ Configuration ⚙️
If your MySQL root password is different from the default, lovingly update these lines in `app.py` (around line 10):
```python
app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'root'
app.config['MYSQL_PASSWORD'] = 'admin'  # 👈 Change this to your actual password!
app.config['MYSQL_DB'] = 'hostel_db'
```

### 4️⃣ Start the Magic! ✨
Run the application gracefully from your terminal:
```bash
python app.py
```

### 5️⃣ Access the App 🎀
Open your favorite web browser and visit:
👉 **[http://127.0.0.1:5000/](http://127.0.0.1:5000/)**

**Test Credentials:**
*   **Admin Access:** Username: `Admin` | Password: `root`
*   **Warden Access:** Username: `warden` | Password: `warden123`

---

<div align="center">
Made with 💖 and a lot of sparkly code! ✨
</div>


