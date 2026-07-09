# 🔁 FFCS Xchanger

## 📌 Project Overview

**FFCS Xchanger** is a web platform designed for students of **Vellore Institute of Technology (VIT)** to easily **swap class slots** with their peers during the FFCS add/drop period. This tool helps avoid the confusion and spam often encountered during manual coordination via WhatsApp or Telegram.

---

## 🚀 Features

- 🔒 User authentication (Signup/Login)
- 📝 Submit swap requests
- 🔍 View existing swap requests
- ✅ Real-time form validations
- 🔗 Easy frontend-backend integration

---

## 🧠 Tech Stack

| Layer      | Tech Used                     |
|------------|-------------------------------|
| Frontend   | React.js, CSS                 |
| Backend    | Node.js, Express.js           |
| Database   | MongoDB (Mongoose ORM)        |
| Hosting    | Netlify (Frontend), Render (Backend) |


## 📂 Project Structure

```
FFCS_Xchanger
│
├── backend
│   ├── models
│   ├── routes
│   ├── middleware
│   ├── server.js
│   └── package.json
│
├── frontend
│   ├── public
│   ├── src
│   └── package.json
│
└── README.md
```

---

## ⚙️ Installation

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/FFCS_Xchanger.git

cd FFCS_Xchanger
```

---

### 2. Install Backend Dependencies

```bash
cd backend

npm install
```

---

### 3. Configure Environment Variables

Create a `.env` file inside the **backend** directory.

```env
MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key

PORT=5000
```

---

### 4. Start Backend

```bash
npm start
```

Server runs on

```
http://localhost:5000
```

---

### 5. Install Frontend Dependencies

```bash
cd ../frontend

npm install
```

---

### 6. Start Frontend

```bash
npm start
```

Application runs on

```
http://localhost:3000
```

---

## 🗄 Database

MongoDB Atlas is used as the cloud database.

Collections include:

- Users
- Slot Requests

---


## 🔒 Authentication Flow

```
Register

↓

Login

↓

JWT Token

↓

Authorized User

↓

Create Slot Request

↓

Stored in MongoDB

↓

Displayed to Other Students
```

---

## 📡 REST API Endpoints

### Authentication

| Method | Endpoint | Description |
|----------|----------|-------------|
| POST | `/api/auth/register` | Register User |
| POST | `/api/auth/login` | Login User |

### Slot Requests

| Method | Endpoint | Description |
|----------|----------|-------------|
| POST | `/api/content` | Create Request |
| GET | `/api/content` | Fetch All Requests |

---

## 🚀 Future Improvements

- Search by Faculty
- Search by Slot
- Automatic Slot Matching
- Email Notifications
- User Dashboard
- Admin Panel
- Real-time Updates using Socket.io
- Docker Support
- Deployment on AWS/Vercel

- Done by Lokeswaran S
