# SecureAuthServer

A secure authentication server built with **Node.js**, **Express**, **PostgreSQL**, and **Passport.js**. This project allows users to register, log in, and manage sessions with cookie-based authentication.

## Description

This application provides a basic authentication flow with the following features:

- **User Registration**: Allows users to create an account using their email and password.
- **User Login**: Allows users to log in securely using email and password.
- **Session Management**: Uses **Express-session** to maintain user sessions across requests.
- **Password Hashing**: Passwords are securely hashed using **bcrypt** before being stored in the database.
- **Session Cookies**: The server sends a session cookie to the user upon successful login to track their authentication state.
- **PostgreSQL**: The app stores user credentials in a **PostgreSQL** database.

The application is designed to be a simple, secure backend for handling user authentication, ideal for use in building secure web applications with Node.js.

## Features

- **Secure User Authentication** with **Passport.js** for both local strategy and session handling.
- **Password Hashing** with **bcrypt** to ensure passwords are stored securely.
- **PostgreSQL** for relational data storage.
- **Express.js** as the backend framework.
- **Session Management** using **express-session** for persistent user login sessions.
- **Cookie-based Authentication** to maintain user login state.

## Installation
The server will start, and the application will be accessible at
https://localhost:3000/

### Prerequisites

To run this project, you need the following installed:

- **Node.js** (preferably the latest LTS version)
- **PostgreSQL** (make sure your database is running)
- **Git** (to clone the repository)

### Steps

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/riiddhii757/SecureAuthServer.git

2. Navigate to the project directory:
cd SecureAuthServer

3. Install the required dependencies:
npm install

4. et up your PostgreSQL database. You need to create a database (e.g., secureauthdb) and configure the credentials in the .env file.

Create the .env file in the root directory and provide the following configuration (replace the placeholders with your actual values):
DB_HOST=localhost
DB_USER=your_username
DB_PASSWORD=your_password
DB_NAME=secureauthdb
SESSION_SECRET=your_secret_key

6. Run Application
npm start

