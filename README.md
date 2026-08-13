TaskFlow is a MERN-stack task management web application built using the MERN Stack (MongoDB, Express.js, React.js, Node.js). It allows users to sign up, log in, and manage their daily tasks with a clean and simple interface — including creating, viewing, updating, and deleting tasks (individually or in bulk).

🚀 Features
🔐 User Authentication – Secure Signup & Login system
➕ Add Task – Create new tasks with a title and description
📋 Task List View – View all tasks in a well-organized table
✅ Bulk Selection & Delete – Select multiple tasks via checkboxes and delete them at once
✏️ Update Task – Edit the title and description of any existing task
❌ Delete Task – Remove individual tasks instantly
🚪 Logout – Securely log out of the application
🖥️ Screenshots
🔑 Login Page
<img width="1366" height="768" alt="login" src="https://github.com/user-attachments/assets/b1f3f889-2e8f-4284-9895-01d1a92208ec" />
🆕 Sign Up Page
<img width="1366" height="768" alt="signup" src="https://github.com/user-attachments/assets/1798c7c8-7999-45a0-8917-cfb3b1058fff" />
📋 Task List
<img width="1355" height="757" alt="list" src="https://github.com/user-attachments/assets/08a4563e-5e1b-48fd-8329-b9c815fca909" />
☑️Select & Delete Tasks
<img width="1366" height="768" alt="deleteone" src="https://github.com/user-attachments/assets/a276ee49-7c58-4b8f-a229-444fcf8d1c96" />
✏️ Update Task
<img width="1366" height="768" alt="updatetask" src="https://github.com/user-attachments/assets/978f1981-8581-451d-8936-acfe463612e2" />
🗑️ Bulk Delete
<img width="1366" height="768" alt="alldell" src="https://github.com/user-attachments/assets/e8a25ccb-d817-4d9d-9b58-43d647ce211c" />
🛠️ Tech Stack

Frontend:

React.js (Vite)
React Router DOM
Axios

Backend:

Node.js
Express.js

Database:

MongoDB (Mongoose)
📂 Project Structure
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
⚙️ Installation & Setup
Clone the repository
bash
   git clone https://github.com/HasnainRiaz/TaskFlow.git
   cd TaskFlow
Setup the Backend
bash
   cd server
   npm install

Create a .env file inside the server folder:

   PORT=3200
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret

Run the backend server:

bash
   npm start
Setup the Frontend
bash
   cd ../client
   npm install
   npm run dev
Open in browser
   http://localhost:5173
📌 API Endpoints (Example)
Method	Endpoint	Description
POST	/api/auth/signup	Register a new user
POST	/api/auth/login	Login existing user
GET	/api/tasks	Get all tasks
POST	/api/tasks	Add a new task
PUT	/api/tasks/:id	Update a task
DELETE	/api/tasks/:id	Delete a task
DELETE	/api/tasks/bulk	Delete multiple tasks
🌟 Future Improvements
Task due dates & priority levels
Task filtering & search
Dark mode UI
Deployment on Render/Vercel
👨‍💻 Author:M.Hasnain Riaz

GitHub: @HasnainRiaz786
