📈 Fin_Track – Stock Portfolio Tracker

Fin_Track is a full-stack MERN application that empowers users to manage their stock portfolios, track real-time trades, maintain a watchlist, and visualize market trends. Whether you're an active trader or a casual investor, Fin_Track simplifies the process of tracking assets and optimizing investments.

🚀 Features
🔐 User Authentication

Secure sign-up and login using JWT-based authentication

💼 Portfolio Management

View live portfolio stats including invested value, returns, and profit/loss

📊 Real-Time Trade Tracking

Log buy/sell trades with automatic updates to holdings

🧾 Trade History

View and manage past transactions with filters and sorting

⭐ Watchlist

Monitor stocks you're interested in without adding them to your portfolio

📈 Data Visualizations

Use Recharts to see trends in performance over time

🌙 Dark Mode

Toggle dark/light theme for better UX

✅ Optimized UX

Clean dashboard with intuitive navigation and responsive layout

🛠️ Tech Stack
Frontend:

React.js

Tailwind CSS

Recharts (for visualizations)

Axios (API calls)

SCSS Modules

Context API (for global state)

Backend:

Node.js

Express.js

MongoDB (MongoDB Atlas)

Mongoose

JWT (Authentication)

dotenv (Secrets Management)

📂 Folder Structure
pgsql
Copy
Edit
fin_track/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── services/
│   └── server.js
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── contexts/
│   │   ├── data/
│   │   ├── charts/
│   │   ├── assets/
│   │   └── App.jsx
│   └── index.html
│
└── README.md
📦 Setup Instructions
🔧 Backend Setup
bash
Copy
Edit
cd backend
npm install
npm run start
Make sure to add a .env file with:

ini
Copy
Edit
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_jwt_secret
🌐 Frontend Setup
bash
Copy
Edit
cd frontend
npm install
npm run dev
📌 Upcoming Features
💹 Integration with real-time stock price APIs (e.g., Alpha Vantage, Finnhub)

🧠 AI-based trade recommendations

📥 Export trade history as CSV

🔔 Price alerts and notifications
