<div align="center">

# 🚀 Contact Form with MongoDB & Admin Authentication

### A Full-Stack Contact Management Web Application

<p>
  <img src="https://img.shields.io/badge/Node.js-Backend-green?style=for-the-badge&logo=node.js"/>
  <img src="https://img.shields.io/badge/Express.js-Server-black?style=for-the-badge&logo=express"/>
  <img src="https://img.shields.io/badge/MongoDB-Database-green?style=for-the-badge&logo=mongodb"/>
  <img src="https://img.shields.io/badge/JWT-Authentication-blue?style=for-the-badge&logo=jsonwebtokens"/>
</p>

A modern **Node.js + Express + MongoDB** application that allows users to submit contact messages and enables authenticated administrators to securely manage and view all submissions through a protected dashboard.

</div>

---

## ✨ Features

- 📝 Contact form submission
- 🔐 Secure admin login authentication
- 🛡️ Protected admin dashboard
- 📂 MongoDB database integration
- 📸 Image, PDF, and file upload support
- 📊 View all submitted messages
- ⚡ REST API with Express.js
- 📱 Responsive web interface

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML** | Frontend Structure |
| **CSS** | Styling |
| **JavaScript** | Client-side Logic |
| **Node.js** | Backend Runtime |
| **Express.js** | Web Framework |
| **MongoDB** | Database |
| **Mongoose** | MongoDB ODM |
| **JWT** | Authentication |
| **Multer** | File Upload |

---

## 📁 Project Structure

```text
tech-company_web/
│
├── models/
│   └── Contact.js
│
├── public/
│   ├── index.html
│   ├── login.html
│   ├── admin.html
│   └── uploads/
│
├── server.js
├── package.json
├── package-lock.json
├── .env
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/jestinkm/tech-company_web.git
cd tech-company_web
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Configure Environment Variables

Create a `.env` file in the root directory:

```env
MONGO_URI=mongodb://127.0.0.1:27017/contactDB
PORT=5000
JWT_SECRET=your_secret_key
```

For MongoDB Atlas:

```env
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/contactDB
PORT=5000
JWT_SECRET=your_secret_key
```

---

## ▶️ Run the Application

Start the server:

```bash
node server.js
```

Open in your browser:

```
http://localhost:5000
```

---

## 🔐 Authentication

The application includes a secure **Admin Login System**.

### Login Request

```json
{
  "email": "admin@example.com",
  "password": "password"
}
```

After successful authentication, the admin can access the protected dashboard and manage all contact submissions.

---

## 📡 API Endpoints

### 📝 Submit Contact Form

**POST** `/contact`

```json
{
  "name": "Jestin",
  "email": "jestin@example.com",
  "message": "Hello!"
}
```

### 🔑 Admin Login

**POST** `/login`

```json
{
  "email": "admin@example.com",
  "password": "password"
}
```

### 📋 Get All Contacts

**GET** `/contacts`

Returns all stored contact messages from MongoDB.

---

## 🖥️ Pages

| Page | Description |
|------|-------------|
| `/` | Contact Form |
| `/login.html` | Admin Login |
| `/admin.html` | Protected Admin Dashboard |

---

## 📸 File Upload Support

Supports uploading:

- 🖼️ Images (JPG, PNG, JPEG)
- 📄 PDF files
- 📁 Documents
- 🎥 Other supported file types

---

## 📊 Admin Dashboard

The dashboard displays:

- 👤 Name
- 📧 Email
- 💬 Message
- 📎 Uploaded File
- 🕒 Date & Time

---

## 🌐 Deployment

- **Backend:** Render
- **Database:** MongoDB Atlas
- **Source Code:** GitHub

---

## 👨‍💻 Author

**Jestin M K**

- GitHub: https://github.com/jestinkm
- LinkedIn: https://www.linkedin.com/

---

<div align="center">

### ⭐ If you found this project useful, please give it a star on GitHub!

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&duration=2500&pause=1000&color=36BCF7&center=true&vCenter=true&width=600&lines=Thank+you+for+visiting!;Happy+Coding!+🚀;Built+with+Node.js+%2B+MongoDB"/>

</div>
