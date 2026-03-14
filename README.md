# 🚀 AI Interview Prep Platform

A **Production-Ready Full Stack Generative AI Job Preparation Platform** that helps users analyze resumes, compare them with job descriptions, detect skill gaps, generate interview questions, and create ATS-optimized resumes.

The system uses **Generative AI** to simulate a real job-preparation workflow where users can upload resumes, paste job descriptions, and receive **AI-generated interview preparation reports**.

---

# 🧠 Core Features

### 🔐 Secure Authentication

* JWT based authentication
* Protected routes
* Token blacklisting for logout security
* Secure API access

### 🤖 AI Interview Preparation

* Resume & Job Description analysis
* Match score calculation
* Technical interview questions
* Behavioral interview questions
* Skill gap detection
* Personalized preparation plan

### 📄 Resume Processing

* Resume upload (PDF/DOCX)
* Resume parsing
* Skill extraction
* Profile summarization

### 📊 ATS Resume Generation

* AI optimized resumes
* Resume improvements suggestions

### 📑 Dynamic Resume PDF Generation

* Resume generated dynamically
* Implemented using **Puppeteer**

### 📂 Real-World Project Architecture

* Feature-based frontend structure
* Service-based backend architecture
* AI service layer
* Context-based state management

---

# 🛠 Tech Stack

### Frontend

* React.js
* Vite
* React Router
* Context API
* Axios
* SCSS

### Backend

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose

### Authentication

* JWT
* Token Blacklisting

### AI Integration

* Gemini AI API

### File Processing

* Multer

### PDF Generation

* Puppeteer

---

# 📂 Project Structure

## Backend

```text
Backend
│
├── src
│   ├── config
│   │   └── database.js
│   │
│   ├── controllers
│   │   ├── auth.controller.js
│   │   └── interview.controller.js
│   │
│   ├── middlewares
│   │   ├── auth.middleware.js
│   │   └── file.middleware.js
│   │
│   ├── models
│   │   ├── user.model.js
│   │   ├── blacklist.model.js
│   │   └── interviewReport.model.js
│   │
│   ├── routes
│   │   ├── auth.routes.js
│   │   └── interview.routes.js
│   │
│   ├── services
│   │   └── ai.service.js
│   │
│   └── app.js
│
├── server.js
├── .env
└── package.json
```

---

## Frontend

```text
Frontend
│
├── src
│
│   ├── features
│   │
│   │   ├── auth
│   │   │   ├── components
│   │   │   │   └── Protected.jsx
│   │   │   │
│   │   │   ├── hooks
│   │   │   │   └── useAuth.js
│   │   │   │
│   │   │   ├── pages
│   │   │   │   ├── Login.jsx
│   │   │   │   └── Register.jsx
│   │   │   │
│   │   │   ├── services
│   │   │   │   └── auth.api.js
│   │   │   │
│   │   │   └── auth.context.jsx
│   │
│   │
│   │   └── interview
│   │       ├── hooks
│   │       │   └── useInterview.js
│   │       │
│   │       ├── pages
│   │       │   ├── Home.jsx
│   │       │   └── Interview.jsx
│   │       │
│   │       ├── services
│   │       │   └── interview.api.js
│   │       │
│   │       ├── style
│   │       │   ├── home.scss
│   │       │   └── interview.scss
│   │       │
│   │       └── interview.context.jsx
│
│   ├── style
│   │   └── button.scss
│
│   ├── App.jsx
│   ├── app.routes.jsx
│   └── main.jsx
│
├── index.html
└── vite.config.js
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/interview-prep-ai.git
cd interview-prep-ai
```

---

# Backend Setup

```bash
cd Backend
npm install
```

Create `.env`

```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
GOOGLE_API_KEY=your_gemini_api_key
```

Run backend

```bash
npm run dev
```

---

# Frontend Setup

```bash
cd Frontend
npm install
npm run dev
```

---

# 🔄 Application Flow

1️⃣ User registers or logs in
2️⃣ JWT authentication token is generated
3️⃣ User uploads resume or writes self description
4️⃣ User pastes job description
5️⃣ AI analyzes candidate profile
6️⃣ System generates:

* Match score
* Technical interview questions
* Behavioral interview questions
* Skill gap analysis
* Personalized preparation roadmap

7️⃣ User can generate **ATS optimized resume PDF**

---

# 🤖 AI System Architecture

The backend **AI service** processes:

```
Resume + Job Description + Self Description
        ↓
Gemini AI Analysis
        ↓
Structured Interview Report
        ↓
Stored in MongoDB
        ↓
Displayed in React Dashboard
```

AI generates:

* Match score
* Technical questions
* Behavioral questions
* Skill gaps
* Preparation plan

All outputs are validated using **Zod Schema** before being stored.

---

# 📈 Future Improvements

* Resume semantic search using vector embeddings
* AI mock interview simulator
* Company specific interview datasets
* Job scraping integration
* Personalized learning dashboard
* Interview progress tracking

---

# 🎯 Use Cases

* Job seekers preparing for interviews
* Resume optimization for ATS systems
* Skill gap identification
* AI powered interview preparation

---

# 👨‍💻 Author

Built as a **production style AI full stack project** demonstrating modern architecture using:

* React
* Node.js
* MongoDB
* Generative AI

---

# ⭐ Support

If you like this project, give it a **star ⭐ on GitHub**.
