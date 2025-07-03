# todo-task-management
# ✅ Todo Task Management Web Application
This is a full-stack Todo Task Management Web App built as part of a hackathon run by [Katomaran](https://www.katomaran.com). It enables users to authenticate with Google, manage personal and shared tasks, and perform CRUD operations with real-time updates and collaboration.

## Live Demo

- 🔗 Frontend: [https://todo-frontend-smvn.onrender.com](https://todo-frontend-smvn.onrender.com)
- 🔗 Backend: [https://todo-backend-vmlw.onrender.com](https://todo-backend-vmlw.onrender.com)

## Demo Video

🎥 Loom video: [Click here to watch the demo](#)  
_Replace the `#` with your Loom video URL._

## Architecture Diagram

 ![architecture](https://github.com/user-attachments/assets/f4a398fa-a2f5-48b3-a314-5cabe6591bf8)
(./architecture.png)

## Tech Stack

| Layer     | Technology                     |
|-----------|--------------------------------|
| Frontend  | React, Bootstrap, Axios        |
| Backend   | Node.js, Express               |
| Auth      | Firebase Authentication (Google OAuth) |
| Database  | MongoDB Atlas (NoSQL)          |
| Hosting   | Render (Frontend + Backend)    |


## Features

- Google Login via Firebase Authentication
- Task CRUD: Create, Read, Update, Delete tasks
- Mark tasks as completed/in-progress
- Task sharing (via user email or UID – extendable)
- Real-time updates (via polling, can upgrade to WebSockets)
- Responsive UI (mobile + desktop)
- Toast alerts for user feedback (e.g., task added, deleted)
- Error handling for API & network failures

## How to Run Locally
## Backend Setup

git clone https://github.com/nandinikamaraj/todo-backend.git
cd todo-backend
npm install

## Create a .env file:
MONGO_URI=mongodb+srv://<your-uri>
PORT=5000
JWT_SECRET=thisisasecret

## Run the server:
node index.js

## Frontend Setup

git clone https://github.com/nandinikamaraj/todo-frontend.git
cd todo-frontend
npm install
npm run dev

## Assumptions

-Only Google login is implemented (GitHub/Facebook skipped for scope).
-Real-time updates are implemented using polling (WebSockets can be added).
-Task sharing feature is assumed to use UID or email (future feature enhancement).
-All services are publicly deployed using free-tier platforms (Render, MongoDB Atlas).
-Rate limiting & validation assumed to be handled manually in Express (basic setup


## Folder Structure

todo-frontend/
├── src/
│   ├── App.jsx        # Main frontend logic
│   ├── firebase.js    # Firebase configuration
│   ├── components/    # UI components (if any)
├── public/
├── .env
├── README.md

todo-backend/
├── routes/
│   ├── taskRoutes.js
│   └── userRoutes.js
├── models/
│   ├── Task.js
│   └── User.js
├── index.js          # Server entry point
├── .env
├── README.md

## Deployment

| Component | Platform      | URL                                                                                |
| --------- | ------------- | ---------------------------------------------------------------------------------- |
| Frontend  | Render        | [https://todo-frontend-smvn.onrender.com](https://todo-frontend-smvn.onrender.com) |
| Backend   | Render        | [https://todo-backend-vmlw.onrender.com](https://todo-backend-vmlw.onrender.com)   |
| DB        | MongoDB Atlas | Cloud-hosted MongoDB                                                               |

## Acknowledgements

This project is a part of a hackathon run by
https://www.katomaran.com
