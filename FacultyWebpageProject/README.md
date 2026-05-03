# Module6_FacultyPagesGroupProject - SPC COP 4504 - Dev Team 2 - 2026

This is a Dev Team 2 group project for the Faculty Web Presence Application. The project began as a static HTML/CSS faculty webpage prototype and was expanded into an interactive, database-driven web application using Flask and MySQL.

The application allows faculty information to be created, read, updated, and managed through a web interface. Faculty profile data is stored in a MySQL database and dynamically displayed on the webpage.

## Contributors

- Matthew W.
- Dannielle M.
- Jacob G.
- LeEric R.

## Project Purpose

This project demonstrates how a static faculty webpage can be transformed into a dynamic web application. The application connects front-end HTML/CSS templates to a MySQL database using Flask routes and server-side logic.

The application supports:

- Dynamic faculty profile display
- Searchable faculty records
- Adding new faculty profiles
- Editing existing faculty profiles
- Course selection for faculty members
- MySQL database interaction
- Server-side form handling
- Parameterized SQL queries
- Confirmation prompts before saving changes
- Warnings when optional fields are cleared
- Warning when leaving the edit page with unsaved changes

## Technologies Used

- HTML5
- CSS3
- Bootstrap 5
- Python
- Flask
- MySQL
- mysql-connector-python
- python-dotenv
- Jinja templates
- Railway hosting
- GitHub version control

## Files Included

```text
FacultyWebpageProject/
│
├── app.py                         # Flask backend routes and database logic
├── facultydatabase_schema.sql      # MySQL database schema and sample setup
├── README.md                       # Project documentation
├── .env                            # Local environment variables, not uploaded to GitHub
│
├── templates/
│   ├── index.html                  # Dynamic faculty home/search page
│   └── edit.html                   # Faculty create/edit form
│
├── static/
│   ├── style.css                   # Main shared CSS
│   ├── spc.css                     # SPC color/theme styling
│   └── images/
│       ├── spc-logo.png            # SPC logo
│       └── user-female.png         # Default faculty profile image
```

## Setup Instructions

1. Clone or download the project git clone <your-repository-url>
- Open the project folder in Visual Studio Code.

2. Create a virtual environment
From the project folder, run:
python -m venv .venv
Activate the virtual environment.
For Windows PowerShell:
.\.venv\Scripts\Activate.ps1

3. Install required packages
- Run: python -m pip install flask python-dotenv mysql-connector-python
- For Railway deployment, install Gunicorn: python -m pip install gunicorn
- Then create or update requirements.txt: python -m pip freeze > requirements.txt

4. Create the MySQL database
- Open MySQL Workbench and run: facultydatabase_schema.sql
Note: This file creates the database tables needed for the application.

5. Create a .env file
- Create a .env file in the main project folder.

6. Run the Flask application locally
- Run: python app.py
- Open the application in a browser: http://127.0.0.1:5000/
- To test the database connection, open: http://127.0.0.1:5000/db-test

