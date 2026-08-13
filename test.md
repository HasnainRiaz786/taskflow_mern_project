# 📝 TaskFlow – Smart Task Manager

TaskFlow is a full-stack task management web application built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js). It allows users to sign up, log in, and manage their daily tasks with a clean and simple interface — including creating, viewing, updating, and deleting tasks (individually or in bulk).

## 🚀 Features

- 🔐 **User Authentication** – Secure Signup & Login system
- ➕ **Add Task** – Create new tasks with a title and description
- 📋 **Task List View** – View all tasks in a well-organized table
- ✅ **Bulk Selection & Delete** – Select multiple tasks via checkboxes and delete them at once
- ✏️ **Update Task** – Edit the title and description of any existing task
- ❌ **Delete Task** – Remove individual tasks instantly
- 🚪 **Logout** – Securely log out of the application

## 🖥️ Screenshots

### 🔑 Login Page
![Login Page](./screenshots/login.png)

### 🆕 Sign Up Page
![Sign Up Page](./screenshots/signup.png)

### 📋 Task List
![Task List](./screenshots/list.png)

### ☑️ Select & Delete Tasks
![Select Tasks](./screenshots/delete-select.png)

### ✏️ Update Task
![Update Task](./screenshots/updatetask.png)

### 🗑️ Bulk Delete
![Bulk Delete](./screenshots/alldelete.png)

> Note: Place your screenshot images inside a `screenshots` folder in the project root, and rename them to match the file names used above (or update the paths accordingly).

## 🛠️ Tech Stack

**Frontend:**
- React.js (Vite)
- React Router DOM
- Axios

**Backend:**
- Node.js
- Express.js

**Database:**
- MongoDB (Mongoose)

## 📂 Project Structure

```
TaskFlow/
├── client/               # React frontend (Vite)
│   ├── src/
│   │   ├── pages/        # Login, Signup, List, Add/Update Task
│   │   ├── components/   # Reusable UI components
│   │   └── App.jsx
│   └── package.json
├── server/               # Express backend
│   ├── models/           # Mongoose schemas
│   ├── routes/           # API routes
│   ├── controllers/      # Route logic
│   └── server.js
└── README.md
```

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/HasnainRiaz/TaskFlow.git
   cd TaskFlow
   ```

2. **Setup the Backend**
   ```bash
   cd server
   npm install
   ```
   Create a `.env` file inside the `server` folder:
   ```
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```
   Run the backend server:
   ```bash
   npm start
   ```

3. **Setup the Frontend**
   ```bash
   cd ../client
   npm install
   npm run dev
   ```

4. **Open in browser**
   ```
   http://localhost:5173
   ```

## 📌 API Endpoints (Example)

| Method | Endpoint            | Description          |
|--------|----------------------|-----------------------|
| POST   | `/api/auth/signup`   | Register a new user  |
| POST   | `/api/auth/login`    | Login existing user  |
| GET    | `/api/tasks`         | Get all tasks         |
| POST   | `/api/tasks`          | Add a new task        |
| PUT    | `/api/tasks/:id`      | Update a task         |
| DELETE | `/api/tasks/:id`      | Delete a task         |
| DELETE | `/api/tasks/bulk`     | Delete multiple tasks |

## 🌟 Future Improvements

- Task due dates & priority levels
- Task filtering & search
- Dark mode UI
- Deployment on Render/Vercel

## 👨‍💻 Author

**Hasnain Riaz**
- GitHub: [@HasnainRiaz](https://github.com/HasnainRiaz)

## 📄 License

This project is licensed under the MIT License.
