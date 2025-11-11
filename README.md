# express-savage-auth

A robust and extensible authentication boilerplate for Express apps

Table of Contents

About

Features

Getting Started

Prerequisites

Installation

Configuration

Usage

Project Structure

Authentication Flow

Customization & Extensibility

Contributing

License

Contact

About

Express-Savage-Auth is a boilerplate for adding user authentication and session management to an Express.js application. It builds on the fundamentals of local authentication, sessions, views, and a modular structure to help you get started quickly with a secure base.

Originally modified from a tutorial by Scotch.io, this version has been cleaned up, modernized, and optimized for easier integration into production-ready apps. 
GitHub

Features

✅ Local username & password authentication

✅ Session support with Express

✅ Modular folder structure (app, config, views, public)

✅ Easily extendable to OAuth, JWT, or other auth strategies

✅ Built with JavaScript + EJS templating

✅ Clear separation of concerns: routes, views, config

Getting Started
Prerequisites

Node.js (version 16.x or higher recommended)

npm or yarn

(Optional) A database or persistent session store if you intend to go beyond in-memory session storage

Installation
git clone https://github.com/AngelBelRoth/express-savage-auth.git  
cd express-savage-auth  
npm install  

Configuration

Copy or rename config/sample.env (if provided) to .env

Set your environment variables, e.g.:

PORT=8080  
SESSION_SECRET=your_super_secret_key  
DB_URI=mongodb://localhost/your_db_name  


If you add a database or session store, configure it in /config (e.g., config/database.js, config/passport.js)

Usage
npm start  


Then open your browser and navigate to http://localhost:8080 (or whatever PORT you configured) to see the app in action. 
GitHub

Project Structure
root/
├─ app/
│   ├─ controllers/
│   ├─ models/
│   ├─ routes/
│   └─ views/
├─ config/
│   ├─ passport.js
│   ├─ database.js
│   └─ …
├─ public/
│   ├─ css/
│   ├─ js/
│   └─ images/
├─ server.js
├─ package.json
└─ README.md


This structure keeps your authentication logic, routing, views and public assets clearly separated and maintainable.

Authentication Flow

User hits the login route → enters credentials

Credentials are validated via Passport (or your selected strategy)

Successful login creates a session stored by Express

User visits protected routes, session middleware verifies logged-in status

Logout destroys session and redirects user

(You can extend this flow with email verification, OAuth2, JWT tokens, etc.)

Customization & Extensibility

Want to swap in JWT instead of sessions? Replace the session middleware in server.js and adjust your auth strategy.

Want to add social login (Google, Facebook, GitHub)? Expand config/passport.js with OAuth strategies.

Want to change the templating engine? Replace EJS files in views/ and adjust the renderer in server.js.

You can easily extract the auth logic as a module for reuse across projects.

Contributing

Contributions are welcome!

Fork the repository

Create a feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request and describe your changes in detail

Please ensure any new code maintains the project’s structure and includes appropriate documentation and tests where relevant.

License

This project is licensed under the MIT License — see the LICENSE
 file for details. 
GitHub

Contact

Created by Angel Bel Roth

Project Link: https://github.com/AngelBelRoth/express-savage-auth
