# Stock-it

A comprehensive stock trading dashboard, built to give you a seamless experience—from tracking real-time market data to managing your portfolio—all wrapped in an intuitive UI.

## Key Technologies

* **React (Vite) + Bootstrap**: Smooth, modern frontend
* **Node.js + Express**: Fast, reliable server
* **MongoDB (Mongoose)**: Flexible, scalable database
* **JWT + Bcrypt.js**: Secure authentication
* **Finnhub API**: Live stock quotes and indices

## Primary Features

* **Secure User Accounts**: Sign up, log in, and log out with HTTP-only cookies
* **Dashboard**: View holdings, open positions, order history, and funds at a glance
* **Watchlist**: Add symbols, see live price updates, and execute buy/sell actions
* **Responsive Design**: Adapts flawlessly across desktop and mobile

## Setup & Local Development

1. **Clone & Remote**

   ```bash
   git clone <your-fork-url>.git
   cd Stock-it
   ```

2. **Backend**

   ```bash
   cd backend
   npm install
   cp .env.sample .env    # fill: PORT, MONGODB_URI, JWT_SECRET, CLIENT_URL
   npm run dev
   ```

3. **Public Frontend**

   ```bash
   cd ../frontend
   npm install
   cp .env.sample .env    # set: REACT_APP_BACKEND_URL, REACT_APP_API_KEY, etc.
   npm run dev
   ```

4. **User Dashboard**

   ```bash
   cd ../dashboard
   npm install
   cp .env.sample .env    # match frontend variables for dashboard
   npm run dev
   ```

## Environment Variables

### backend/.env

```
PORT=3002
MONGODB_URI=mongodb+srv://<user>:<pass>@cluster0.mongodb.net/stock-it-db
JWT_SECRET=your_super_secret
CLIENT_URL=http://localhost:*YOUR_FRONTEND_PORT*
```

### frontend/.env & dashboard/.env

```
REACT_APP_BACKEND_URL=http://localhost:3002
REACT_APP_DASHBOARD_URL=http://localhost:*DASHBOARD_PORT*
REACT_APP_API_KEY=<your_finnhub_api_key>
```

## API Routes

| Path         | Method | Purpose                     |
| ------------ | ------ | --------------------------- |
| `/signup`    | POST   | Register a new user         |
| `/login`     | POST   | Authenticate and set cookie |
| `/logout`    | POST   | Clear user session cookie   |
| `/verify`    | GET    | Check active user session   |
| `/holdings`  | GET    | Fetch current holdings      |
| `/positions` | GET    | Retrieve open positions     |
| `/orders`    | POST   | Submit a new trade order    |

## Project Layout

```
stock-it/
├── backend/     # Express server & MongoDB models
│   ├── controllers/
│   ├── middleware/
│   └── index.js
├── frontend/    # Public site (login & signup)
├── dashboard/   # Private user interface
│   ├── components/
│   └── styles/
└── README.md    # This document
```

## Screenshot Gallery

![Homepage Sketch](./screenshots/home.png)
![Sign Up](./screenshots/signup.png)
![Main Dashboard](./screenshots/dashboard.png)

## Acknowledgements

* Market data powered by [Finnhub.io](https://finnhub.io)
* UI components courtesy of Bootstrap

## Maintainer

**Your Name** — Full-stack Developer
License: MIT © 2025
