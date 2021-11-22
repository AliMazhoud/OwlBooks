# Project 1

Course name: Web Programming with Python and JavaScript <br>


## Youtube: <a href = 'https://youtu.be/B3SLGNpt-Zc' </a>

# `App name:` Owl Books

``Breif description:`` Book Review application made with flask. First you need to register and then login .After registration and logged into the website you can seach for books, see the reviews and submit your own review.

Technology used:
HTML, CSS, JAVASCRIPT, BOOTSTRAP, PYTHON, FLASK, SQLALCHEMY, POSTGRESQL


Book API used:
goodreads.com 

Server used:
heroku.com 

## How to use this app:

1. Clone this repositiory  or Download Source files
2. Run ```pip install -r requirements.txt``` in your terminal/CMD window to make sure that all of the necessary Python packages (Flask and SQLAlchemy, for instance) are installed.
3. Set an environmental variable to connect with database.
    <br> Varialbe name must be: ``"DATABASE_URL"``
    <br> Varialbe value will be: ``"...your database uri ..."``,  ``"export DATABASE_URL="uri"``
4. Run ```python imports.py``` to create user,books and reveiws table in database and to insert 5000 books data from books.csv
5. Run ```python application.py``` to run the app
6. Done

## Features:

**Login:** If user go to root url first it will check if the user is already signed in or not using the session. If not then app will show the login page otherwise app will take the user to the account page without asking him to login everytime. When login page apprears and user input his email and password - app will compare the informations with informations that are already saved in database. If the username and password match then user wiil be logged in and  allowed to go to account page otherwise error message will show.

**Registration:** New user can register on the website. Before registration app will check if there is already any account registered with the same email. If no account found than app will register the account in the website.

**Logout:** Users can log out from the website by clicking on the logout button.

**Admin page:** To view the admin page user must log in first. In the admin page users can see his account information and reviewed books list with a search box.

**Search:** By clicking the search menu  button Users can search books by Title or Author or Year or ISBN number. If user submit the keyword in the search bar a search result table will appear with book list with that information.

**Book page:** By clicking a book title from  the search result users can view information about that book. Statical information will come from goodread.com api and reviews data will come from my website database.

**Api:** go to /isbn , where isbn is the book's isbn that you want to get the json informations
