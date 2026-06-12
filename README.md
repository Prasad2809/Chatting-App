<div align="center">

# 💬 Real-Time Chat Application

### A Modern Full-Stack Chat App with Real-Time Messaging, Authentication & Docker Support

[![Node.js](https://img.shields.io/badge/Node.js-v14+-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Latest-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![Socket.io](https://img.shields.io/badge/Socket.io-Latest-010101?style=for-the-badge&logo=socketdotio&logoColor=white)](https://socket.io/)
[![JWT](https://img.shields.io/badge/JWT-Secured-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)](https://jwt.io/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.0-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

<br/>

[🚀 Live Demo](http://localhost:8080/) 

</div>

---

## 📋 Table of Contents

- [📖 About The Project](#-about-the-project)
- [✨ Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Prerequisites](#️-prerequisites)
- [🚀 Getting Started](#-getting-started)
- [🐳 Docker Setup](#-docker-setup)
- [📝 Environment Variables](#-environment-variables)
- [🔌 API Endpoints](#-api-endpoints)
- [📸 Screenshots](#-screenshots)
- [👤 Author](#-author)

---

## 📖 About The Project

A production-ready, real-time chat application built from the ground up
using modern web technologies. Designed for scalability, security,
and a smooth user experience — this project demonstrates a full-stack
implementation with containerized services using Docker.

This project showcases:

- 🔐 Secure Authentication using JSON Web Tokens (JWT)
- ⚡ Real-time Communication powered by Socket.io
- 🐳 Containerized Deployment using Docker and Docker Compose
- 🎨 Modern UI built with React, TailwindCSS and DaisyUI
- 📦 Scalable Architecture ready for Kubernetes orchestration

---

## ✨ Features

| Feature                | Description                                              |
|------------------------|----------------------------------------------------------|
| 💬 Real-Time Messaging | Instant messaging using WebSockets via Socket.io         |
| 🔐 JWT Authentication  | Secure login and registration with token-based auth      |
| 👤 Profile Management  | Upload and update profile pictures                       |
| 🟢 Online Status       | See who is online or offline in real time                |
| 📱 Responsive Design   | Works on all screen sizes — desktop, tablet, mobile      |
| 🐳 Docker Support      | Fully containerized for easy setup and deployment        |
| 🔒 Secure Architecture | Protected routes, encrypted passwords, secured APIs      |
| 🎨 Modern UI           | Clean and intuitive interface with DaisyUI components    |

---

## 🛠️ Tech Stack

### 🖥️ Frontend

| Technology       | Purpose                    |
|------------------|----------------------------|
| ⚛️ React 18      | UI Framework               |
| 🎨 TailwindCSS   | Utility-first CSS styling  |
| 🌼 DaisyUI       | Pre-built UI components    |
| 🐻 Zustand       | Lightweight state management |
| 🔌 Socket.io Client | Real-time communication |

### ⚙️ Backend

| Technology      | Purpose                        |
|-----------------|--------------------------------|
| 🟢 Node.js      | JavaScript runtime             |
| 🚂 Express.js   | Web application framework      |
| 🍃 MongoDB      | NoSQL database                 |
| 🔌 Socket.io    | WebSocket server               |
| 🔑 JWT          | Authentication & Authorization |
| 🔒 Bcrypt       | Password hashing               |

### 🐳 DevOps & Infrastructure

| Technology        | Purpose                          |
|-------------------|----------------------------------|
| 🐳 Docker         | Containerization                 |
| 📦 Docker Compose | Multi-container orchestration    |
| 🌐 Nginx          | Web server and reverse proxy     |
| ☸️ Kubernetes     | Container orchestration (planned)|

---

## 📁 Project Structure
full-stack-chatApp/
│
├── 📁 backend/
│   │
│   ├── 📁 src/
│   │   │
│   │   ├── 📁 controllers/
│   │   │   ├── 📄 auth.controller.js
│   │   │   └── 📄 message.controller.js
│   │   │
│   │   ├── 📁 models/
│   │   │   ├── 📄 user.model.js
│   │   │   └── 📄 message.model.js
│   │   │
│   │   ├── 📁 routes/
│   │   │   ├── 📄 auth.route.js
│   │   │   └── 📄 message.route.js
│   │   │
│   │   ├── 📁 middleware/
│   │   │   └── 📄 auth.middleware.js
│   │   │
│   │   ├── 📁 lib/
│   │   │   ├── 📄 db.js
│   │   │   ├── 📄 socket.js
│   │   │   └── 📄 utils.js
│   │   │
│   │   └── 📄 index.js
│   │
│   ├── 📄 .env                  ← ⚠️ NEVER push to GitHub
│   ├── 📄 .env.example          ← ✅ Safe to push
│   ├── 📄 .gitignore
│   ├── 📄 Dockerfile
│   └── 📄 package.json
│
│
├── 📁 frontend/
│   │
│   ├── 📁 src/
│   │   │
│   │   ├── 📁 components/
│   │   │   ├── 📁 ui/
│   │   │   │   ├── 📄 Button.jsx
│   │   │   │   ├── 📄 Input.jsx
│   │   │   │   └── 📄 Avatar.jsx
│   │   │   │
│   │   │   ├── 📁 chat/
│   │   │   │   ├── 📄 ChatContainer.jsx
│   │   │   │   ├── 📄 ChatHeader.jsx
│   │   │   │   ├── 📄 ChatInput.jsx
│   │   │   │   └── 📄 MessageBubble.jsx
│   │   │   │
│   │   │   ├── 📁 sidebar/
│   │   │   │   ├── 📄 Sidebar.jsx
│   │   │   │   └── 📄 UserList.jsx
│   │   │   │
│   │   │   ├── 📄 Navbar.jsx
│   │   │   └── 📄 OnlineStatus.jsx
│   │   │
│   │   ├── 📁 pages/
│   │   │   ├── 📄 HomePage.jsx
│   │   │   ├── 📄 LoginPage.jsx
│   │   │   ├── 📄 RegisterPage.jsx
│   │   │   └── 📄 ProfilePage.jsx
│   │   │
│   │   ├── 📁 store/
│   │   │   ├── 📄 useAuthStore.js
│   │   │   ├── 📄 useChatStore.js
│   │   │   └── 📄 useThemeStore.js
│   │   │
│   │   ├── 📁 hooks/
│   │   │   ├── 📄 useSocket.js
│   │   │   └── 📄 useOnlineStatus.js
│   │   │
│   │   ├── 📁 lib/
│   │   │   ├── 📄 axios.js
│   │   │   └── 📄 utils.js
│   │   │
│   │   ├── 📄 App.jsx
│   │   ├── 📄 main.jsx
│   │   └── 📄 index.css
│   │
│   ├── 📁 public/
│   │   ├── 📄 favicon.ico
│   │   └── 📄 logo.png
│   │
│   ├── 📄 Dockerfile
│   ├── 📄 nginx.conf
│   ├── 📄 index.html
│   ├── 📄 tailwind.config.js
│   ├── 📄 vite.config.js
│   └── 📄 package.json
│
│
├── 📁 screenshots/
│   ├── 🖼️ login.png
│   ├── 🖼️ chat.png
│   └── 🖼️ profile.png
│
│
├── 📄 docker-compose.yml
├── 📄 .gitignore
└── 📄 README.md📄 README.md # Project documentation




