# Todo App

A full-stack Todo App built with React (frontend) and Node.js with Express (backend) using MongoDB for data storage. The app allows users to register, login, create, read, update, and delete tasks. JWT-based authentication ensures users only have access to their own tasks.

## Features

- **User Authentication**: Register, login, and logout functionality with JWT tokens.
- **Task Management**: Create, read, update, and delete tasks.
- **Protected Routes**: Users can only access tasks if they are authenticated.
- **Responsive UI**: Built using React and Material-UI for better user experience.

## Technologies Used

### Frontend
- React
- Axios
- Material-UI
- React Router

### Backend
- Node.js
- Express
- MongoDB
- Mongoose
- JWT (JSON Web Token)
- CORS
- bcrypt


##Project Structure

todoapp/
│
├── backend/                   # Backend code (Express, MongoDB)
│   ├── controllers/           # Controllers handling business logic (TaskController, UserController)
│   ├── middleware/            # Authentication middleware (protect.js)
│   ├── models/                # Database schemas (Task, User)
│   ├── routes/                # Route definitions (taskRoutes, userRoutes)
│   ├── config/                # Database connection (db.js)
│   ├── .env                   # Environment variables (MONGO_URI, JWT_SECRET)
│   ├── server.js              # Main Express server file
│   ├── package.json           # Backend dependencies and scripts
│   └── Procfile               # File for deploying backend on Heroku
│
├── frontend/                  # Frontend code (React)
│   ├── public/                # Public assets (index.html)
│   ├── src/                   # React application source code
│   │   ├── components/        # React components (Login, Register, TodoList, TaskForm)
│   │   ├── context/           # React Context API for managing authentication state (AuthContext.js)
│   │   ├── App.js             # Main React App component with routing
│   │   ├── index.js           # React DOM rendering
│   │   └── package.json       # Frontend dependencies and scripts
├── README.md                  # Project documentation (this file)
└── .gitignore                 # Files to ignore in version control


##Backend Setup

Navigate to the backend directory and install dependencies
Create a .env file in the backend directory with the following variables:
MONGO_URI=<Your MongoDB connection string>
JWT_SECRET=<Your Secret Key>
 Start the backend server


##Frontend Setup
Navigate to the frontend directory and install dependencies
Start the React development server

Connecting Frontend and Backend
axios.post('http://localhost:5000/api/users/login', { email, password });
