# HMS Pro - Hostel Management System

HMS Pro is a web-based Hostel Management System built with Python (Flask) and MySQL. It provides a comprehensive dashboard to manage students, rooms, attendance, fees, and user roles (Admin/Warden).

## Project Structure and File Details

Here is a breakdown of all the files in the project and what they do:

- **`app.py`**: The core backend application file. It uses the Flask framework to serve the frontend pages (`index.html` and `login.html`) and provides RESTful API endpoints (`/api/login`, `/api/users`, `/api/students`, `/api/rooms`, `/api/attendance`, `/api/fees`, etc.) to interact with the database. It handles routing, session management, and database queries.
- **`schema.sql`**: The database schema definition file. It contains the SQL commands to create the `hostel_db` database and all the required tables: `users`, `hostels`, `rooms`, `students`, `attendance`, and `fees`. It also includes initial mock data to get started.
- **`index.html`**: The main frontend dashboard page. It provides the user interface for administrators and wardens to view statistics, manage students, assign rooms, mark attendance, and track fees.
- **`login.html`**: The authentication page. It contains the UI for users to log in with their credentials and role (Admin or Warden).
- **`assets/`**: Contains the static assets for the frontend.
  - **`assets/css/style.css`**: The stylesheet that defines the visual design, layout, and styling of the web pages, ensuring a clean and modern user interface.
  - **`assets/js/app.js`**: The frontend JavaScript file. It handles client-side logic, such as making asynchronous API requests (using `fetch`), updating the DOM dynamically, handling form submissions, and managing UI state dynamically.

## Prerequisites

Before running the project, ensure you have the following installed:
- Python 3.x
- MySQL Server
- `pip` (Python package installer)

## Dependencies

The project uses the following Python packages:
- `Flask`
- `flask-mysqldb`

You can install them using pip:
```bash
pip install Flask flask-mysqldb
```

## Setup and Installation

### 1. Database Setup
1. Open your MySQL client or command line.
2. Run the `schema.sql` script to create the database, tables, and insert initial mock data.
```bash
mysql -u root -p < schema.sql
```
*(If your MySQL credentials differ, adjust the command accordingly.)*

### 2. Configure Database Credentials
Open `app.py` and update the MySQL configuration section to match your local database credentials (if they are different from the defaults):
```python
app.config['MYSQL_HOST'] = 'localhost'
app.config['MYSQL_USER'] = 'root'
app.config['MYSQL_PASSWORD'] = 'admin' # Change this to your MySQL password
app.config['MYSQL_DB'] = 'hostel_db'
```

### 3. Run the Application
Start the Flask development server by running:
```bash
python app.py
```
The server will start, usually accessible at `http://127.0.0.1:5000`.

## How to Use the Project

1. **Login**: Open your browser and navigate to `http://127.0.0.1:5000`. You will be presented with the login screen.
   - Initial Admin credentials: Username: `Admin`, Password: `root`
   - Initial Warden credentials: Username: `warden`, Password: `warden123`
2. **Dashboard**: Once logged in, you will be directed to the dashboard.
   - The top section displays key statistics (Total Students, Available Rooms, Present Today, Pending Fees).
3. **Manage Students**: Add new students, assign them to rooms, and view existing student records.
4. **Manage Attendance**: Mark daily attendance (Present/Absent/Outing) for students.
5. **Manage Fees**: Update fee status for students.
6. **Manage Users (Admin only)**: Administrators can add new users (Admins or Wardens) to the system.

## Troubleshooting
- **Database Connection Error**: Double-check that MySQL is running and the credentials in `app.py` are correct.
- **Missing Module Error**: Ensure you have installed the required Python packages (`Flask` and `flask-mysqldb`) in your active Python environment.
