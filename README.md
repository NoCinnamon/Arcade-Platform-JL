# Project over view:

![ Demo](./assets/demo-screen-2.png)

🕹️ Arcade Platform
A full-stack web arcade featuring classic games like Minesweeper and Snake, complete with a persistent global leaderboard and user authentication.

🚀 Features
User Accounts: Secure signup and login using Bcrypt encryption.

Global Leaderboard: Compete for high scores stored in MongoDB.

Classic Games: Fully playable Snake and Minesweeper built with Vue.js.

Responsive Design: Playable on various screen sizes.

🛠️ Tech Stack
Frontend: Vue.js + Vite

Backend: Node.js + Express

Database: MongoDB Atlas

Authentication: JWT / Express-Session & Bcrypt

📦 Getting Started
Prerequisites
Node.js (v18 or higher recommended)

A MongoDB Atlas account and cluster.

1. Backend Setup
   Navigate to the backend directory:

Bash
cd backend
Install dependencies:

Bash
npm install
Create a .env file and add your MongoDB connection string:

Plaintext
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.xxxx.mongodb.net/arcade?retryWrites=true&w=majority
PORT=3000
Start the server:

Bash
node main-express.js 2. Frontend Setup
Open a new terminal tab and navigate to the frontend directory:

Bash
cd frontend
Install dependencies:

Bash
npm install
Start the development server:

Bash
npm run dev
Open your browser to the URL shown in the terminal (usually http://localhost:5173).

🖥️ Project Structure
Plaintext
├── backend/
│ ├── main-express.js # Main server entry point
│ ├── model.js # MongoDB schemas (User, Score)
│ └── .env # Environment variables (private)
├── frontend/
│ ├── src/ # Vue components and game logic
│ ├── public/ # Static assets
│ └── vite.config.js # Vite configuration
└── README.md
