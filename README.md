---

## URL Shortener with User Authentication - Flask Application

This project is a *Flask-based URL shortener* application that includes *user authentication* and URL management. Registered users can log in, create short URLs for long links, and track the number of clicks for each shortened URL.

### Key Technologies:
- *Flask*: Web framework
- *Flask-SQLAlchemy*: Database management
- *Flask-Login*: User authentication
- *Flask-Migrate*: Database migrations
- *Werkzeug Security*: Password hashing for secure login

### Features:
- *User Registration & Authentication*: Users can register, log in, and log out securely.
- *URL Shortening*: Generate short URLs for any long URL.
- *Click Tracking*: Track how many times each shortened URL is clicked.
- *Responsive Dashboard*: Manage all shortened URLs from a personal dashboard.
- *Error Handling*: User-friendly feedback for invalid logins, duplicate registrations, and non-existent URLs.

### Project Setup:

1. *Clone the Repository*:
   bash
   git clone https://github.com/your-username/url-shortener-flask.git
   cd url-shortener-flask
   

2. *Set up a Virtual Environment*:
   bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   

3. *Install Dependencies*:
   bash
   pip install -r requirements.txt
   

4. *Set up the Database*:
   bash
   flask db init
   flask db migrate
   flask db upgrade
   

5. *Run the Application*:
   bash
   python app.py
   
   Navigate to http://127.0.0.1:5000 in your browser.

### How It Works:
- *User Registration*: Users sign up with an email and password, which is securely hashed using werkzeug.security.generate_password_hash.
- *Login*: Registered users can log in and access their dashboard.
- *Dashboard*: 
   - Shorten new URLs by entering the original URL.
   - View all shortened URLs with their respective click counts.
- *Redirect*: Visiting a shortened URL redirects the user to the original URL and updates the click count.
- *Logout*: Users can log out to securely terminate their session.

### Tech Stack:
- *Flask*: Python web framework.
- *SQLite*: Database for storing users and URLs.
- *Flask-SQLAlchemy*: ORM for handling the database.
- *Flask-Login*: Manages user sessions.
- *Flask-Migrate*: Handles database migrations.

### Possible Improvements:
- *Email Verification*: Add email verification for enhanced security.
- *Custom Short URLs*: Allow users to create personalized short URLs.
- *Analytics*: Provide detailed statistics for each URL, such as user location and device data.
  
---
