### EDUcheck
EDUcheck is a comprehensive web application designed to facilitate online education management. It provides a robust platform for teachers and students to interact, manage courses, assignments, and communicate in real-time.

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

## Deploy to Vercel

The repository includes `main.py` and `vercel.json` for a Flask serverless deployment. Vercel uses temporary SQLite storage at `/tmp/educheck.db` and temporary upload storage, so data is not durable across cold starts. Face recognition is optional in the serverless build because its native dependency is not included in `requirements.txt`; the face endpoints return a safe failure response when it is unavailable. Real-time Socket.IO connections and durable uploads should use a production server, managed database, and object storage.

```bash
npx vercel login
npx vercel --prod
```
