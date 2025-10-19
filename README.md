<h1 align="center">📝 BlogApp</h1>

<p align="center">
  <b>A full-stack blogging platform built with React, Node.js, Express, MongoDB, and Gemini AI API.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Frontend-React-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/Backend-Node.js-green?style=flat-square" />
  <img src="https://img.shields.io/badge/Database-MongoDB-brightgreen?style=flat-square" />
  <img src="https://img.shields.io/badge/AI-Gemini%20API-purple?style=flat-square" />
  <img src="https://img.shields.io/badge/Version-1.0.0-blueviolet?style=flat-square" />
  <img src="https://img.shields.io/badge/Live-Demo-orange?style=flat-square" />
  
</p>

---

## 🚀 Overview  
**BlogApp** is a modern blogging platform that allows users to create, read, update, and delete blog posts.  
It integrates **Gemini AI API** to assist with content generation, summaries, and suggestions, providing a smarter blogging experience.  

Built with a React frontend and a Node.js/Express backend, it offers a seamless experience for both readers and writers.

---

## ✨ Key Features  
- 📝 **Create, Edit, and Delete Blog Posts**  
- 📖 **View Blog Posts by Category**  
- 🔍 **Search for Blogs**  
- 🤖 **Gemini AI API** – Generate content or summaries automatically  
- 🔐 **User Authentication**  
- 📱 **Responsive Design**  

---

## 🧩 Project Structure 

    BlogApp/
    │
    ├─ client/ # React frontend
    │ ├─ src/
    │ │ ├─ components/
    │ │ ├─ pages/
    │ │ ├─ services/
    │ │ └─ App.js
    │ └─ package.json
    │
    ├─ server/ # Node.js + Express backend
    │ ├─ controllers/
    │ ├─ models/
    │ ├─ routes/
    │ ├─ config/
    │ ├─ services/ # Gemini AI API integration
    │ ├─ server.js
    │ └─ .env
    │
    └─ README.md


---

## ⚙️ Installation & Setup  

### 1️⃣ Clone the repository  
      ```bash
      git clone https://github.com/GarvRastogi05/BlogApp.git
      cd BlogApp

2️⃣ Backend Setup
    
    cd server
    npm install

3️⃣ Setup Environment Variables

Create a .env file inside the server/ directory and add:

     # JWT Secret
    JWT_SECRET = 'secret@2025'
    
    # Admin Credentials
    ADMIN_EMAIL = "admin@example.com"
    ADMIN_PASSWORD = "admin1234"
    
    # MongoDB
    MONGODB_URI = "Enter your mongodb_uri"
    
    # ImageKit
    IMAGEKIT_PUBLIC_KEY = 'Enter your Imagekit public key'
    IMAGEKIT_PRIVATE_KEY = 'Enter your Imagekit private key'
    IMAGEKIT_URL_ENDPOINT = 'Enter your Imagekit URI endpoint'
    
    # Gemini API Key
    GEMINI_API_KEY = 'Enter your api key'
    

Start the backend server:

    npm run start

4️⃣ Frontend Setup

        cd ../client
        npm install
        npm start

🤖 Gemini AI API Integration :

1. Used for content generation, suggestions, and automated summaries.
2. The backend connects to Gemini AI API using your API key.
   
Example usage in your server code:

    import axios from "axios";
    
    const response = await axios.post(
      "https://api.gemini.ai/v1/generate",
      { prompt: "Write a blog intro about AI in 100 words" },
      { headers: { Authorization: `Bearer ${process.env.GEMINI_API_KEY}` } }
    );
    
    console.log(response.data);

  🧠 Tech Stack :
  
| Category       | Technology       |
| -------------- | ---------------- |
| Frontend       | React.js         |
| Backend        | Node.js, Express |
| Database       | MongoDB          |
| Authentication | JWT              |
| AI API         | Gemini AI        |


🧪 Usage

1. Navigate to the homepage to view all blog posts.
2. Click on a post to read more.
3. Log in to create, edit, or delete your own posts.
4. Use the AI features for auto-generating content or summaries.

👨‍💻 Contributing

Contributions are welcome!
1. Fork the repository
2. Create a feature branch (git checkout -b feature/new-feature)
3. Commit changes (git commit -m "Added a new feature")
4. Push to your branch (git push origin feature/new-feature)
5. Create a Pull Request

<p align="center">💙 Developed by <b>Garv Rastogi</b></p> ```
