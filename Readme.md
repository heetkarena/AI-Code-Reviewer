# 🧠 AI Code Reviewer with Gemini API (React + Node.js)

This is a full-stack AI-powered code reviewer that allows developers to submit code and receive intelligent reviews using **Google's Gemini API**. Built using **React** for the frontend and **Node.js (Express)** for the backend, organized in an MVC architecture.

---

## 🧩 Features
## Overview

This project is a full-stack application that leverages the Google Gemini API to provide automated code reviews. The frontend is developed using React, while the backend utilizes Node.js with Express, following the Model-View-Controller (MVC) architectural pattern. The application is designed for maintainability, scalability, and ease of use.

---

## Key Features

* Integrated live code editor with syntax highlighting (PrismJS and React Simple Code Editor)
* Automated code review powered by Gemini LLM
* Feedback rendered in Markdown for readability
* Modular MVC backend structure for clear separation of concerns
* Responsive user interface styled with Tailwind CSS

---
* 💻 Live code editor (PrismJS + React Simple Code Editor)
* 🤖 Code review using Gemini LLM
* 📋 Markdown-rendered feedback
* 💡 Clean, maintainable codebase using MVC pattern
* 🎨 Tailwind CSS-powered responsive design

---

## 📁 Folder Structure

```
root/
├── Frontend/               # React frontend
│   ├── src/
│   │   ├── App.jsx
│   │   └── index.js
│   └── public/
│       └── index.html
│   └── tailwind.config.js
├── Backend/               # Node.js backend (MVC)
│   ├── controllers/
│   │   └── reviewController.js
│   ├── routes/
│   │   └── reviewRoutes.js
│   ├── services/
│   │   └── geminiService.js
│   └── app.js
├── .env
├── package.json
└── README.md
```

---

## 🌐 API Endpoint

### POST `/api/review`

**Purpose:** Submits code for AI review.

**Request:**

```json
{
  "code": "function sum(a, b) { return a + b; }"
}
```

**Response:**

```json
"### AI Review\n- The function is clear and concise.\n- Consider adding parameter validation.\n..."
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone 
cd ai-code-reviewer
```

---

### 2. Install Dependencies

#### Backend

```bash
cd Backend
npm install
```

#### Frontend

```bash
cd ../Frontend
npm install
```

---

### 3. Environment Setup

In `Backend/.env`:

```env
GEMINI_API_KEY=your_gemini_api_key_here
```

---

### 4. Start the App

Open two terminals:

**Terminal 1: Backend**

```bash
cd Backend
node app.js
```

**Terminal 2: Frontend**

```bash
cd Frontend
npm run dev  
```

## 🚨 Disclaimer

* Do **not** expose your Gemini API key in client-side code.
* Use for educational or internal testing purposes.
* Refrain from submitting sensitive or proprietary code.

## 👤 Author

Made by Heet Karena

---

## 📄 License

Licensed under the [MIT License](LICENSE).
