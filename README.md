# express-savage-auth  
_A robust and extensible authentication boilerplate for Express.js apps_

![Node.js](https://img.shields.io/badge/node-%3E%3D16-brightgreen?style=flat-square)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)

---

## 📖 Table of Contents  
- [About](#about)  
- [Features](#features)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
  - [Configuration](#configuration)  
  - [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Authentication Flow](#authentication-flow)  
- [Customization & Extensibility](#customization--extensibility)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## About  
**express-savage-auth** is a modernized boilerplate for quickly adding **user authentication** and **session management** to your Express.js projects.  

It’s built to be modular, extendable, and easy to customize — perfect for starting new projects that need secure, scalable login functionality.  

Originally inspired by a Scotch.io tutorial, this version has been **cleaned, structured, and upgraded** for today’s best practices.  

> Ideal for: developers who want a solid Express auth base without reinventing the wheel.  

**Repository:** [github.com/AngelBelRoth/express-savage-auth](https://github.com/AngelBelRoth/express-savage-auth)

---

## ✨ Features  
- 🔐 Local username/password authentication  
- 💾 Session support with `express-session`  
- 🧩 Modular file structure for clean scalability  
- 🖥️ EJS templating and ready-to-use views  
- ⚙️ Easy integration with Passport.js strategies (Local, OAuth, etc.)  
- 🔄 Extendable to JWT, OAuth2, or API-based systems  
- 🧱 Clear separation of app, config, routes, and views  

---

## 🏁 Getting Started  

### Prerequisites  
- [Node.js](https://nodejs.org/) v16+  
- npm or yarn  
- Optional: MongoDB (or another database) for persistent session storage  

### 💻 Installation  
```bash
# Clone the repository
git clone https://github.com/AngelBelRoth/express-savage-auth.git

# Move into the project directory
cd express-savage-auth

# Install dependencies
npm install

# Start the development server
npm run dev

