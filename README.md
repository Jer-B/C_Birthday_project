# Birthday Reminder Web Application

## About the project

This is a web application built in Python using the Flask framework. It's designed to help you keep track of the birthdays of people you know, ensuring you never forget them.

## How to use

1. Add people's names and their corresponding birthday dates.

## Understanding

- `application.py`: This file contains the code for the Flask web application. It includes one route (`/`) that handles both POST and GET requests. When the `/` route is requested via GET, it renders the `index.html` template. When requested via POST, the user is redirected back to `/` via GET.

- `birthdays.db`: This is an SQLite database with a `birthdays` table, including columns for `id`, `name`, `month`, and `day`. You can insert new rows into this table using the web application.

- `static/styles.css`: This directory contains the CSS code for the web application. You can modify this file to customize the appearance of your application.

- `templates/index.html`: This HTML file is rendered when users visit your web application.

## Installation

To set up the required dependencies, follow these steps:
Be sure to change pip for pip3 if necessary.

1. Clone this repository to your local machine.

2. Create a virtual environment (optional but recommended):
   
   Using `virtualenv` (if not installed, run `pip install virtualenv`):
   
   ```bash
   virtualenv venv
   ```
   Or using venv (Python 3.3+):
   ```bash
   python -m venv venv
   ```
3. If using a virtual environment (Step 2), activate it:
   - On Windows:
   ```bash
   venv\Scripts\activate
   ```
   - On macOS and Linux:
   ```bash
   source venv/bin/activate
   ```
   
4. Install the required packages from requirements.txt:
   ```bash
   pip install -r requirements.txt
   ```
This will set up the necessary packages for the project.

## Testing

To test the Flask application, run the following command in your terminal while in your the directory:
   ```bash
   flask run
   ```
   This will start a web server that serves the Flask application. You can then access the application by opening your web browser and navigating to http://localhost:5000.
   
Enjoy using the Birthday Reminder Web Application!