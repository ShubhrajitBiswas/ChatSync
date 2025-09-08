# ChatSync 💬🚀

**ChatSync** is a real-time chat application that allows users to register, log in, and chat with other online users seamlessly. It features **real-time messaging**, **profile updates**, and **image uploads via Cloudinary**. Built with **React, Node.js, MongoDB, and Socket.io**, it provides a modern chat experience.

---

## 📸 Screenshots  
**Home / Chat Page**  
![App Screenshot](./screenshot.png)  

---

## 📌 Features

### 👤 User Side
- 🔑 Sign up and log in securely  
- 🗨️ Real-time messaging with online users  
- 📁 Update profile with image upload  
- 🖼️ Upload images using Cloudinary  
- ⚡ Responsive and interactive UI  

### 🛠️ Backend
- 🔐 JWT-based authentication  
- 💾 MongoDB database with Mongoose  
- ⚡ Real-time communication via Socket.io  
- ☁️ Cloudinary integration for media uploads  
- 📊 Tracks online users  

---

## 🛠️ Tech Stack  

### Frontend
- React.js  
- Tailwind CSS  
- Vite  
- Axios  
- Zustand (state management)  
- React Hot Toast  

### Backend
- Node.js  
- Express.js  
- MongoDB + Mongoose  
- Socket.io  
- JWT Authentication  
- Cloudinary for media  

---

## 💾 Database
- MongoDB Atlas (cloud) or local MongoDB instance  
- Collections: `users`, `messages`  

---

## 🚀 How to Run Locally  

### Prerequisites
- Node.js  
- MongoDB instance (local or Atlas)  
- Cloudinary account  

### 🔧 Setup Instructions  

#### 1. Clone the Repository
- git clone https://github.com/ShubhrajitBiswas/ChatSync.git
- cd ChatSync
#### 2. Backend Setup
- cd backend
- npm install
- Create a `.env` file inside `/backend`:
- MONGODB_URI=your_mongodb_connection_string
- PORT=5001
- JWT_SECRET=your_jwt_secret
- CLOUDINARY_CLOUD_NAME=your_cloud_name
- CLOUDINARY_API_KEY=your_api_key
- CLOUDINARY_API_SECRET=your_api_secret
- NODE_ENV=development
- Run the backend:
- npm run start

#### 3. Frontend Setup
- cd ../frontend
- npm install

Create a `.env` file inside `/frontend`:


---

## 🌐 Deployment  

- Backend deployed on Render: [https://chatsync-e2b6.onrender.com](https://chatsync-e2b6.onrender.com)  
- Frontend deployed on Render: [https://chatsync-frontend.onrender.com](https://chatsync-frontend.onrender.com)  

Make sure `VITE_API_URL` in the frontend `.env` points to your deployed backend URL.  

---

## ⚡ Features in Action
- Real-time chat with online user detection  
- Upload and display profile pictures using Cloudinary  
- JWT authentication for secure access  
- React-based SPA with responsive design  

---

## 📂 Folder Structure
```
ChatSync/
├── backend/
│   └── src/
│       ├── controllers/
│       ├── lib/
│       ├── models/
│       ├── routes/
│       └── index.js
├── frontend/
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── components/
│       ├── pages/
│       ├── store/
│       ├── lib/
│       ├── App.jsx
│       └── main.jsx
│   └── tailwind.config.js
└── README.md
```

---

## 🔧 Notes
- Ensure MongoDB IP whitelist includes your server IP (or `0.0.0.0/0` for testing).  
- Frontend `.env` `VITE_API_URL` must match backend URL.  
- Refreshing SPA routes requires backend or hosting to serve `index.html` for all unknown routes.  
