
---


# 🔐 Secure User Authentication - MERN Stack

A secure full-stack authentication system built with the MERN stack and Mailtrap for email verification. Includes user signup, login, email verification, password reset, and protected routes.

---

## 🚀 Features
- User Registration & Login
- JWT Authentication & Protected Routes
- Email Verification (via Mailtrap API)
- Forgot & Reset Password
- Password Hashing (bcryptjs)
- Session Handling & Logout
- Fully Responsive UI with TailwindCSS + DaisyUI

---

## ⚙ Tech Stack
**Frontend:** React.js, Axios, React Router, TailwindCSS, DaisyUI  
**Backend:** Node.js, Express.js, MongoDB, JWT, bcryptjs  
**Email Service:** Mailtrap Email Sending API

---

## 🛠 Setup

### 🔗 Clone & Install
bash
git clone https://github.com/your-username/mern-auth-app.git

cd mern-auth-app
`

### 📦 Backend

bash

cd backend

npm install


📁 Create `.env` file:

env

PORT=5000

MONGO_URI=your_mongo_uri

JWT_SECRET=your_secret

MAILTRAP_TOKEN=your_mailtrap_token

MAILTRAP_ENDPOINT=https://send.api.mailtrap.io/api/send
```

```bash
npm run dev


### 💻 Frontend

bash
cd ../frontend
npm install
npm start


---

## 🔗 API Routes

| Method | Endpoint                         | Description        |
| ------ | -------------------------------- | ------------------ |
| POST   | /api/auth/register               | Register new user  |
| GET    | /api/auth/verify/\:token         | Email verification |
| POST   | /api/auth/login                  | User login         |
| POST   | /api/auth/logout                 | Logout             |
| POST   | /api/auth/forgot-password        | Request reset      |
| POST   | /api/auth/reset-password/\:token | Reset password     |

---

## 📧 Mailtrap Setup

1. Visit [mailtrap.io](https://mailtrap.io)
2. Go to **Email Sending → Integration**
3. Click **Manage Credentials → Generate Token**
4. Assign domain & view email permissions
5. Copy token to `.env` as `MAILTRAP_TOKEN`

---



