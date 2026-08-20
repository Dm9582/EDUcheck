# EDUcheck

**EDUcheck** is a Flask-based education management platform that lets teachers and students interact online in real time. Teachers can create courses, generate class codes, take attendance, and run live chat sessions, while students can enroll with a code, join classes, submit assignments, and chat with classmates. The project is organized into modules: `app/routes/` splits `auth`, `teacher`, `student`, `chat`, and `attendance` views; `app/models.py` defines the SQLAlchemy data layer (User, Course, Assignment, AttendanceSession, etc.); `app/templates/` holds Jinja2 pages across `auth`, `dashboards`, `courses`, `attendance`, `chat`, and `assignments` folders; and `app/utils/` houses helpers for face recognition and attendance logic.

## Features
- User Authentication : Secure login and registration for students and teachers.
- Course Management : Teachers can create and manage courses, generate class codes, and handle enrollments.
- Assignment System : Create, submit, and track assignments with due date countdowns.
- Real-time Chat : Integrated chat system for direct communication between students and teachers.
- Attendance Tracking : Manage and monitor student attendance records.
- Announcements : Teachers can post announcements for their classes.
- Profile Management : Users can update and manage their profiles.

## Technologies Used
- Frontend : HTML, CSS, JavaScript, Socket.IO
- Backend : Flask, Flask-SQLAlchemy, Flask-SocketIO
- Database : SQLite
- Authentication : Flask-Login
- Real-time Communication : Flask-SocketIO
## Installation
1. Clone the repository.
2. Install dependencies using pip install -r requirements.txt .
3. Set up the database using Flask-Migrate.
4. Run the application with flask run .

## Live Demo

The current Vercel deployment is available at [educheck-rust.vercel.app](https://educheck-rust.vercel.app).


