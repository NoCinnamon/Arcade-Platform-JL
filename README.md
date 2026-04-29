# 🕹️ Arcade Platform

A full-stack MEVN-style arcade web app where users authenticate, play **Minesweeper** and **Snake**, and submit scores to a persistent global leaderboard.

### ⚡ Quick Start

```bash
# Terminal 1 (backend)
cd backend
npm install
node main-express.js

# Terminal 2 (frontend)
cd frontend
npm install
npm run dev
```

Then open: `http://localhost:5173`

### 📸 Project Preview

![Login Page](./assets/login.png)
![Home Page](./assets/home-page.png)

<details>
  <summary><b>View More Gameplay Screenshots</b></summary>
  
  **Snake**
  ![Snake Game Over](./assets/snake-lost.png)
  
  **Minesweeper**
  ![MineSweeper Gameplay](./assets/mineSweeper-5boms.png)
  ![MineSweeper Lost](./assets/MS-lost.png)
  ![Score Record Option](./assets/MS-lost-score-record-option.png)
  ![Minefield Revealed](./assets/MS-lost-show-bom.png)
  ![Win Record Option](./assets/MS-win-score-record-option.png)
  
  **Leaderboard**
  ![Global Leaderboard](./assets/leaderBoard.png)
</details>

---

## 🚀 Features

- **Implemented secure authentication:** Built signup/login flows using Express sessions and Bcrypt password hashing.
- **Built a persistent leaderboard system:** Stored and served game scores from MongoDB for cross-user ranking.
- **Developed two browser games:** Delivered fully playable Snake and Minesweeper with Vue.js components.
- **Shipped a responsive interface:** Optimized gameplay and layouts for desktop and smaller screens.

## 🛠️ Tech Stack

- **Frontend:** Vue.js + Vite
- **Backend:** Node.js + Express
- **Database:** MongoDB Atlas
- **Authentication:** Express-Session + Bcrypt

---

## 📦 Getting Started

### Prerequisites

- **Node.js** (v18 or higher recommended)
- A **MongoDB Atlas** account and cluster.

### 1. Backend Setup

Navigate to the backend directory and install dependencies:

```bash
cd backend
npm install
```

Create a `.env` file in `backend/`:

```env
MONGO_URI=your_mongodb_connection_string
SESSION_SECRET=your_secret_key
PORT=3000
```

Start the backend server:

```bash
node main-express.js
```

You should see:
`Server running at http://0.0.0.0:3000`

---

### 2. Frontend Setup

Open a **new terminal**, then run:

```bash
cd frontend
npm install
npm run dev
```

Vite will print a local URL, usually:
`http://localhost:5173`

---

### 3. Run the App

1. Open the frontend URL in your browser.
2. Register a new account or log in.
3. Play Snake or Minesweeper.
4. Scores are saved to MongoDB and shown on the leaderboard.

---

### 4. API/Port Notes

- Frontend calls backend at `http://localhost:3000`
- Backend port is controlled by `PORT` in `backend/.env` (default `3000`)
- If you change backend port, update frontend API base URL accordingly

---

### 5. Troubleshooting

- **MongoDB connection error:** Verify `MONGO_URI` and Atlas network access.
- **Session/auth issues:** Make sure `SESSION_SECRET` is set.
- **Frontend cannot reach backend:** Confirm backend is running on port `3000`.
- **Node errors:** Check your Node version with `node -v` (use v18+).
