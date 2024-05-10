# Flask-Authentication



Flask User Authentication and Secrets Management

Overview
This Flask application demonstrates user authentication and secrets management using Flask-SQLAlchemy and Flask-Login. Users can register, log in, access a secret page, and log out. Registered users have access to download a file.

Features
* User Registration: Users can register with a unique email, password, and name. Passwords are securely hashed using PBKDF2.
* User Login: Registered users can log in using their email and password. Passwords are verified securely.
* Session Management: Flask-Login manages user sessions, allowing access to protected routes only when logged in.
* Secrets Page: A secret page is accessible only to logged-in users, displaying the user's name.
* File Download: Logged-in users can download a file from the server.

Technologies Used
* Flask: A lightweight web framework for Python.
* Flask-SQLAlchemy: Integrates SQLAlchemy with Flask for database operations.
* Flask-Login: Provides user session management and authentication.
* Werkzeug: A WSGI utility library for Python.
* SQLite: A lightweight SQL database engine, used for storing user information.

Usage

1. Install dependencies: pip install -r requirements.txt
2. Run the Flask application: python app.py
3. Access the application in your browser at http://localhost:5000

Notes
* The secret key for Flask sessions is stored securely. Ensure to replace 'secret-key-goes-here' with your own secret key in app.py.
* This application uses SQLite as the database. For production use, consider using a more robust database like PostgreSQL or MySQL.
