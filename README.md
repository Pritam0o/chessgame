# 🧠 Real-Time Multiplayer Chess Game

A real-time, two-player chess game built with **Node.js**, **Socket.IO**, **Express**, and **Vanilla JavaScript**, using **chess.js** for game logic and EJS for rendering the frontend.

<img width="960" height="540" alt="image" src="https://github.com/user-attachments/assets/f343a8c1-ee72-4cd2-9f12-3e19b9c21dd6" />

---

## 🕹️ Features

- Real-time multiplayer over WebSockets (Socket.IO)
- Drag-and-drop chess UI
- Legal move validation using `chess.js`
- Auto board flipping for black player
- Spectator support (if both players are already playing)

---

## 📁 Project Structure

project/
│
├── public/
│ └── js/
│ └── chessgame.js # Frontend logic (UI + Socket events)
│
├── views/
│ └── index.ejs # Main HTML (rendered by Express)
│
├── app.js # Server logic (Express + Socket.IO)
├── package.json
└── README.md # This file

yaml
Copy
Edit

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/chessgame.git
cd chessgame
2. Install Dependencies
bash
Copy
Edit
npm install
3. Run the Server
bash
Copy
Edit
node app.js
The app runs at http://localhost:3000

👥 How It Works
First user to join becomes White

Second user becomes Black

Further users are Spectators

Server validates all moves using chess.js

Each player can only move when it's their turn

🛠️ Tech Stack
Backend: Node.js, Express, Socket.IO

Frontend: EJS, HTML, CSS (Tailwind), JavaScript

Game Logic: chess.js

🧩 Known Limitations
No persistence (refresh resets the game)

No user authentication

No UI feedback for invalid moves yet



🙌 Credits
chess.js for validating and simulating chess logic

Socket.IO for enabling real-time play

Icons: Unicode chess characters ♔♕♖♘♗♙

