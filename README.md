# 👨‍💼 Employee Management App

A simple and clean **Employee Management System** built with **Node.js**, **Express.js**, **MongoDB**, and **Pug** for templating. This app allows you to **add**, **edit**, **view**, and **delete** employee records through a user-friendly web interface.

## ✨ Features

- Add new employees with details like ID, Name, Email, Mobile No, Gender, Department, and Location.
- View a table of all employees.
- Edit employee information.
- Delete an employee record with confirmation.

## 🧱 Project Structure

```
employee-management/
├── models/
│   └── Employee.js          # Mongoose schema for employee
├── views/
│   ├── index.pug            # Employee list page
│   ├── edit-employee.pug    # Edit form view
│   ├── new-employee.pug     # (assumed for adding new employee)
├── public/
│   └── style.css            # CSS styles
├── server.js                # Main application logic
├── package.json             # Project metadata
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/employee-management.git
cd employee-management
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run MongoDB Locally

Ensure MongoDB is installed and running locally at:

```
mongodb://127.0.0.1:27017/employeesDB
```

### 4. Start the Server

```bash
node server.js
```

### 5. Open in Browser

Visit: [http://localhost:3000](http://localhost:3000)

## 📋 Routes Summary

| Method | Route          | Description                    |
|--------|----------------|--------------------------------|
| GET    | /              | List all employees             |
| GET    | /new           | Show form to add employee      |
| POST   | /add           | Add a new employee             |
| GET    | /edit/:id      | Show form to edit employee     |
| POST   | /update/:id    | Update employee by ID          |
| GET    | /delete/:id    | Delete employee by ID          |

## 📦 Dependencies

- express
- mongoose
- pug
- body-parser

Install all dependencies via:

```bash
npm install express mongoose pug body-parser
```

## 🎨 UI Styling

The app uses a custom `style.css` file for modern, responsive UI design, including hover effects, table styling, buttons, and form layouts.

