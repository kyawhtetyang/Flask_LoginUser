# Flask User Management CRUD

**Project Overview**
A simple Flask web app for managing users with login, roles, and CRUD operations.  
Built as part of the *Flask Fundamentals* learning series.

---

## Features
- User login/logout with session timeout (30 mins)
- Role-based access: `admin`, `editor`, `viewer`
- Full CRUD operations (create, read, update, delete)
- User profile: username, age, email, bio, and profile picture
- User search (by username)
- REST API endpoints (`/api/users`, `/api/users/<username>`)
- Upload and display profile pictures (stored in `static/uploads`)

---

## Folder Structure
```bash
Flask_UserLogin_CRUD/
├─ data.py                 # Handles user data including email, bio, and profile picture
├─ app.py                  # Main Flask application entry
├─ auth.py                 # Authentication routes (login, logout)
├─ users.py                # User management (CRUD, search, profile)
├─ static/
│  └─ uploads/             # Stores uploaded profile images
└─ templates/
   ├─ base.html
   ├─ login.html
   ├─ logout.html
   ├─ hello.html
   ├─ users.html             # User list with profile links
   ├─ create_user.html       # Form to add new user
   ├─ search_results.html    
   ├─ profile.html           
   ├─ edit_user.html
   └─ confirm_delete.html

```
---

## Setup
### Local Python Environment
```bash
cd ~/Flask_UserLogin_CRUD/
pip install -r requirements.txt
python app.py

# Flask runs on http://127.0.0.1:5000 by default
```
