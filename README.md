# Dining Social Platform Web Project

This project is a web application for a dining social platform, developed as part of Introduction to Databases course. It allows users to create and browse dining events, communicate, rate chefs, and more.

## Project Structure

```
README.md
requirements.txt
server.py
static/
    index.css
    index.js
    login.css
    message.css
    navbar.css
    profile.css
    signup.css
    survey.css
    images/
        person.png
templates/
    anotherfile.html
    index.html
    login.html
    message.html
    navbar.html
    profile.html
    signup.html
    survey.html
```

## Features

- User registration, login, logout
- Create dining events (survey form)
- Browse and filter dining events (multiple filter options)
- User profile page (email, tags, ratings, reviews, posted events)
- Messaging between users
- Event reviews and ratings
- Responsive frontend pages

## Quick Start

1. **Install dependencies**

   Make sure you have Python 3. Install required packages:

   ```sh
   pip install -r requirements.txt
   ```

2. **Configure the database**

   Edit `server.py` and set your database URI:

   ```python
   DATABASEURI = "postgresql://<USER>:<PASSWORD>@<DB_SERVER>/<DB_NAME>"
   ```

3. **Run the project**

   ```sh
   python server.py
   ```

   The default port is 8112. Visit [http://localhost:8112](http://localhost:8112) in your browser.

4. **Command line help**

   ```sh
   python server.py --help
   ```

## Main Dependencies

- Flask
- SQLAlchemy
- psycopg2-binary
- click
- python-dotenv

See `requirements.txt` for details.

## File Overview

- `server.py`: Main backend service, routes and database logic
- `static/`: Frontend static resources (CSS, JS, images)
- `templates/`: Jinja2 template files for all pages
- `requirements.txt`: Python dependencies
- `README.md`: Project documentation

## Database Overview

Uses PostgreSQL with main tables:

- `users`: User information
- `surveys_fill_out`: Dining event information
- `reviews_about`: Reviews and ratings
- `message_send`: User messages
- `filters`, `filter`: Filtering options and relations

---
