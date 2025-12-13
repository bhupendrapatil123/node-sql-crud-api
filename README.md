# 🧑‍💻 Node SQL CRUD API (Node.js + Express + MySQL + EJS)

A simple User Management Web App built with Node.js, Express, MySQL, and EJS.
Perform basic CRUD operations — view, edit, and update user details with a clean UI.

---

## 🚀 Features

- View total number of users
- Display all user records in a table
- Edit and update username (with password verification)
- Clean EJS templates for rendering pages
- Uses `method-override` for HTTP PATCH requests

---

## 🗂️ Project Structure

project-folder/
│
├── views/
│ ├── home.ejs
│ ├── showusers.ejs
│ └── edit.ejs
│
├── index.js
├── schema.sql
├── package.json
└── README.md


---

## ⚙️ Technologies Used

- **Backend:** Node.js, Express.js  
- **Database:** MySQL (using `mysql2` package)  
- **Templating Engine:** EJS  
- **Utilities:** Faker.js, Method-Override  

---

## 🛠️ Installation and Setup

### 1. Clone the Repository
git clone https://github.com/bhupendrapatil123/node-sql-crud-api.git
cd node-sql-crud-api

### 2. Install Dependencies
      npm install

### 3. Create the Database
    Open MySQL and run:
       CREATE DATABASE delta_app;
       USE delta_app;
       SOURCE schema.sql;

### 4. Start the Server
       node index.js

# Available Routes:
| Route            | Method | Description                          |
| ---------------- | ------ | ------------------------------------ |
| `/`              | GET    | Show total user count                |
| `/user`          | GET    | List all users                       |
| `/user/:id/edit` | GET    | Edit a specific user                 |
| `/user/:id`      | PATCH  | Update username after password check |





