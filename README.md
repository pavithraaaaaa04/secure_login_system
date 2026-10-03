# Secure Login System

A Flask-based web application implementing secure user authentication with hashed passwords, SQL injection protection, and session management.

Features
- User registration and login with hashed passwords (werkzeug.security, bcrypt-style hashing)
- SQL injection protection via parameterized queries
- Session-based authentication with logout functionality
- SQLite database for persistent user storage

How It Works
1. Users register with a username and password
2. Passwords are hashed before being stored in the database (never stored as plain text)
3. On login, the entered password is checked against the stored hash
4. A session is created on successful login, allowing access to a protected dashboard
5. Logging out clears the session

Project Structure
secure_login_app/
app.py
setup_db.py
users.db
templates/
register.html
login.html
dashboard.html
## ▶️ How to Run
1. Install Flask: `pip install flask`
2. Run `setup_db.py` once to create the database
3. Run `app.py`
4. Open `http://127.0.0.1:5000` in your browser

## ⚠️ Note
This project was built and tested successfully (Flask server confirmed running via terminal), as part of a Cyber Security internship task focused on secure authentication practices and web application security fundamentals.

## 🎓 Project Context
Built as part of a Cyber Security internship mini project to gain hands-on understanding of authentication security, password hashing, and protection against common web vulnerabilities like SQL injection.
