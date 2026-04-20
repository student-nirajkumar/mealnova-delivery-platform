# MealNova

**MealNova** is a next-level, production-style **Real-Time Food Delivery System** built with the **MERN stack**. It is inspired by modern food delivery platforms, but it is designed as a real-world full-stack application with live tracking, role-based access, secure authentication, cloud image uploads, and online payments.

---

## 🚀 Project Overview

MealNova is built to handle the complete food ordering flow:

* users can browse food items and place orders
* owners can manage shops and menu items
* delivery partners can handle assigned deliveries
* the app supports real-time tracking and live order updates
* payments are handled securely through a gateway

This project is strong for:

* college submission
* internship portfolio
* resume showcase
* MERN stack practice
* full-stack interview discussion

---

## ✨ Key Features

* **User authentication** with secure login and registration
* **Google authentication** for faster sign-in
* **JWT-based authorization**
* **Role-based access control** for:

  * User
  * Owner
  * Delivery Partner
* **Cart and checkout flow**
* **Order placement and order history**
* **Real-time map tracking** using **Google Maps + Socket.io**
* **Razorpay payment integration**
* **Password reset using email OTP**
* **Shop management** for owners
* **Food item management** with edit/update/delete support
* **Image upload handling** using **Multer + Cloudinary**
* **Responsive frontend UI**
* **Scalable backend structure**

---

## 🧠 What Makes This Project Next-Level

This is not just a simple CRUD project. It includes advanced features that reflect real product development:

* real-time communication
* secure user sessions
* cloud storage for images
* payment processing
* map-based live tracking
* separate dashboards for different roles
* reusable backend architecture

---

## 🛠 Tech Stack

### Frontend

* React.js
* Vite
* Tailwind CSS
* Redux Toolkit
* Firebase
* Socket.io Client
* Google Maps API

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* Socket.io
* Razorpay SDK
* Nodemailer
* Multer
* Cloudinary

### Tools

* Git & GitHub
* ESLint
* Environment variables
* REST APIs

---

## 📁 Folder Structure

```bash
mealnova/
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   │   ├── deliveryAssignment.model.js
│   │   ├── item.model.js
│   │   ├── order.model.js
│   │   ├── shop.model.js
│   │   └── user.model.js
│   ├── public/
│   ├── routes/
│   ├── utils/
│   ├── .env
│   ├── .gitignore
│   ├── index.js
│   ├── package.json
│   ├── package-lock.json
│   └── socket.js
├── frontend/
│   ├── public/
│   ├── src/
│   ├── .env
│   ├── .gitignore
│   ├── eslint.config.js
│   ├── firebase.js
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── README.md
│   └── vite.config.js
└── README.md
```

---

## 📌 Backend Structure Explained

### `config/db.js`

Handles MongoDB database connection.

### `controllers/`

Contains the main business logic for users, shops, food items, orders, and delivery flow.

### `middlewares/`

Used for authentication, error handling, and request protection.

### `models/`

Contains MongoDB schemas for:

* users
* shops
* items
* orders
* delivery assignments

### `routes/`

Defines API endpoints for the application.

### `utils/`

Contains helper functions such as email, token, cloud upload, or file handling utilities.

### `socket.js`

Handles real-time socket connection for live delivery tracking.

### `index.js`

Main backend entry file.

---

## 📌 Frontend Structure Explained

### `src/`

Contains the main React application source code.

### `firebase.js`

Used for Firebase-related integration if required.

### `vite.config.js`

Vite configuration file for frontend development.

### `public/`

Static assets.

### `index.html`

Main HTML entry point.

---

## 🔐 Authentication Flow

MealNova supports secure login and access control using:

* email/password authentication
* Google one-tap login
* JWT token-based protection
* role-based route handling
* password reset through email OTP

---

## 💳 Payment Flow

The app supports a full checkout experience:

1. user adds food items to cart
2. user proceeds to checkout
3. payment is processed using Razorpay
4. order is stored in the database
5. order status is updated in real time

---

## 📍 Real-Time Tracking Flow

The live tracking system works using:

* Google Maps for location display
* Socket.io for live communication
* delivery updates between server and client
* order movement visibility for users

---

## 🖼 Image Upload Flow

Food item and shop images are handled using:

* **Multer** for file upload
* **Cloudinary** for cloud storage
* local file cleanup after upload

This keeps the backend organized and storage efficient.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/mealnova.git
cd mealnova
```

### 2. Install backend dependencies

```bash
cd backend
npm install
```

### 3. Install frontend dependencies

```bash
cd ../frontend
npm install
```

---

## 🔐 Environment Variables

### Backend `.env`

```env
PORT=5000
MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLIENT_URL=http://localhost:5173
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
SMTP_HOST=your_smtp_host
SMTP_PORT=your_smtp_port
SMTP_USER=your_email
SMTP_PASS=your_email_password
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

### Frontend `.env`

```env
VITE_API_URL=http://localhost:5000
VITE_GOOGLE_CLIENT_ID=your_google_client_id
VITE_FIREBASE_API_KEY=your_firebase_key
```

---

## ▶️ Running the Project

### Start backend

```bash
cd backend
npm run dev
```

### Start frontend

```bash
cd frontend
npm run dev
```

---

## 🧪 Available Scripts

### Backend

* `npm run dev` → run backend in development mode
* `npm start` → run backend in production mode

### Frontend

* `npm run dev` → start frontend development server
* `npm run build` → create production build
* `npm run preview` → preview production build

---

## 🌐 Deployment

You can deploy this project using:

* **Frontend:** Vercel / Netlify
* **Backend:** Render / Railway
* **Database:** MongoDB Atlas

---

## 🔒 Security Highlights

* passwords are hashed before storage
* JWT protects private routes
* environment variables keep secrets safe
* file uploads are handled securely
* role-based logic protects owner and delivery pages

---

## 🚀 Future Improvements

* coupon and discount system
* ratings and reviews
* push notifications
* admin analytics dashboard
* dark mode
* order cancellation flow
* advanced filtering and search
* multi-language support

---

## 👨‍💻 Author

**Niraj Kumar**

---

## ⭐ Support

If you like this project, give it a star on GitHub and use it as a strong portfolio project.
