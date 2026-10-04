<div align="center">

# Gursha Server

**The Node.js backend powering Gursha, a TikTok-inspired mobile social media application.**

A REST API built with Express and MongoDB to handle users, short-form video posts, authentication, and chat-related functionality for the Gursha mobile application.

![Node.js](https://img.shields.io/badge/Node.js-18-339933?logo=node.js)
![Express](https://img.shields.io/badge/Express.js-4-000000?logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-7-47A248?logo=mongodb)
![JWT](https://img.shields.io/badge/Auth-JWT-000000?logo=jsonwebtokens)

</div>

---

## 📖 Overview

Gursha Server provides the backend infrastructure for the Gursha mobile application.

It exposes REST API endpoints for user accounts, posts, authentication, following, and chat functionality, while using MongoDB for persistent data storage.

---

## ✨ Core Features

* 🔐 **Authentication** — User registration, login, and JWT-based authentication
* 👤 **User Management** — Profiles, user information, and following relationships
* 🎥 **Post Management** — Create, retrieve, update, and delete video posts
* ❤️ **Social Features** — Following and user interactions
* 💬 **Chat API** — Backend support for chat functionality
* 🗄️ **MongoDB** — Persistent application data using Mongoose
* 🔒 **Password Security** — Password hashing with bcrypt

---

## 🏗️ Architecture

The server follows a simple Express-based REST API architecture.

```text
gursha-server/
├─ models/       → MongoDB / Mongoose models
├─ routes/       → API route handlers
├─ utils/        → Shared utilities
├─ validations/  → Request validation
├─ index.js      → Application entry point
└─ package.json  → Project configuration
```

### API Routes

| Route    | Purpose                            |
| -------- | ---------------------------------- |
| `/users` | Authentication and user management |
| `/posts` | Video post management              |
| `/chats` | Chat-related functionality         |

---

## 🚀 Getting Started

### Prerequisites

* Node.js
* MongoDB
* Git

### Installation

```bash
git clone https://github.com/jonathanadel-dev/gursha-server.git
cd gursha-server
npm install
```

### Environment Variables

Create a `.env` file and configure the MongoDB connection:

```env
MONGO_URL=your_mongodb_connection_string
```

### Run the server

Development:

```bash
npm run dev
```

Production:

```bash
npm start
```

The server runs on port `4000` by default.

---

## 🛠️ Tech Stack

| Layer            | Technology           |
| ---------------- | -------------------- |
| Runtime          | Node.js              |
| Framework        | Express.js           |
| Database         | MongoDB              |
| ODM              | Mongoose             |
| Authentication   | JSON Web Tokens      |
| Password Hashing | bcryptjs             |
| Middleware       | CORS, Morgan, dotenv |
| API Format       | REST                 |

---

## 📌 Project Status

Gursha Server is the backend component of the Gursha social media application and is maintained alongside the Gursha mobile client.

---

<div align="center">

Built by **Jonathan Adel**

</div>
