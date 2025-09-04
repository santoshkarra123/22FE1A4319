# 🚀 Affordmed URL Shortener

A full-stack **URL Shortener** project built as part of the **Affordmed
Campus Drive task**.\
It provides a simple way to shorten long URLs, track usage stats, and
even generate QR codes.

------------------------------------------------------------------------

## 🌟 Features

-   🔗 **Shorten Long URLs** into unique short codes.\
-   📊 **Statistics Page** showing number of created links.\
-   🗑️ **Delete Short URLs** directly from the list.\
-   📱 **QR Code Generator** for every shortened link.\
-   🧭 **Smooth Navigation** with Material UI Navbar.\
-   📝 **Logging Middleware** in backend for tracking all requests.\
-   🎨 **Modern UI** with Material UI + custom CSS animations.

------------------------------------------------------------------------

## 🏗️ Tech Stack

### Frontend

-   React 18\
-   Material UI (MUI v5)\
-   Axios\
-   qrcode.react

### Backend

-   Node.js + Express\
-   Logging Middleware (custom + optional `morgan`)\
-   shortid (for unique short codes)\
-   CORS + dotenv

------------------------------------------------------------------------

## 📂 Project Structure

    affordmed-url-shortener/
    │
    ├── backend/                 # Express server
    │   ├── middleware/          # Logging middleware
    │   ├── server.js            # API routes
    │   └── package.json
    │
    ├── frontend/                # React app
    │   ├── src/
    │   │   ├── components/      # Navbar, UrlForm, UrlList, Stats
    │   │   ├── App.js
    │   │   ├── App.css
    │   │   └── index.js
    │   ├── public/
    │   └── package.json
    │
    └── README.md

------------------------------------------------------------------------

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository

``` bash
git clone https://github.com/your-username/affordmed-url-shortener.git
cd affordmed-url-shortener
```

### 2️⃣ Setup Backend

``` bash
cd backend
npm install
npm run dev   # Starts Express server with Nodemon
```

By default, backend runs at:\
👉 `http://localhost:5000`

### 3️⃣ Setup Frontend

``` bash
cd ../frontend
npm install
npm start
```

Frontend runs at:\
👉 `http://localhost:3000`

------------------------------------------------------------------------

## 🔍 API Endpoints (Backend)

  Method   Endpoint     Description
  -------- ------------ ------------------------
  POST     `/shorten`   Create a short URL
  GET      `/:code`     Redirect to long URL
  GET      `/stats`     Get all shortened URLs

------------------------------------------------------------------------

## 📸 Screenshots

👉 *(Add screenshots of your app here for extra polish --- Homepage,
Stats page, QR Code example)*

------------------------------------------------------------------------

## 🧾 Logging Example

Logs are stored in `logs/server.log`:

    [2025-09-04T10:20:31.234Z] POST /shorten 200 - 45ms
    [2025-09-04T10:21:02.876Z] GET /stats 200 - 12ms

------------------------------------------------------------------------

## 👨‍💻 Author

-   **Your Name**\
-   📧 youremail@example.com\
-   🌐 [LinkedIn](https://www.linkedin.com/) \|
    [GitHub](https://github.com/)

------------------------------------------------------------------------

## 📜 License

This project is licensed under the **MIT License**.
