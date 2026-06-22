# MeetOnMemory

<div align="center">

### AI-Powered Meeting Memory & Management Platform

Transform meetings, discussions, and organizational knowledge into a searchable and structured repository using AI.

![React](https://img.shields.io/badge/React-19-blue)
![Node.js](https://img.shields.io/badge/Node.js-20-green)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green)
![Express](https://img.shields.io/badge/Express.js-Backend-black)
![Vite](https://img.shields.io/badge/Vite-Frontend-purple)
![Gemini](https://img.shields.io/badge/Google-Gemini-blue)

</div>

---

## Overview

MeetOnMemory is a full-stack AI-powered platform built to address the challenge of meeting management, policy tracking, and institutional knowledge retention.

Organizations often lose valuable information because meeting notes, decisions, policies, and discussions are scattered across emails, documents, and chats. MeetOnMemory centralizes this information and makes it searchable through AI-powered semantic search and automated meeting summaries.

---

## Problem Statement

Develop a centralized system to manage meetings, events, and policy records while improving:

* Knowledge retention
* Accountability
* Documentation
* Information retrieval
* Organizational transparency

MeetOnMemory provides a single platform where organizations can store, manage, search, and analyze meeting-related information.

---

# Features

## Meeting Management

* Create meetings
* Manage meeting details and agenda
* Track meeting history
* Organize discussions in one place

## AI Meeting Summaries

* Generate Minutes of Meeting (MoM)
* Extract key discussion points
* Capture decisions
* Generate structured summaries using Google Gemini

## Semantic Search

Search organizational knowledge using natural language queries.

Examples:

```text
What was decided about the education policy?

Show discussions related to AI implementation.

Find previous meetings discussing recruitment.
```

Powered by:

* Pinecone Vector Database
* Embeddings
* AI-based similarity search

## Policy Repository

* Upload policy documents
* Maintain policy versions
* Store organizational records
* Centralized policy management

## Reports & Analytics

* Meeting statistics
* Policy activity tracking
* Organization insights
* Visual dashboards

## Authentication & Security

* JWT Authentication
* Protected Routes
* Password Hashing (bcrypt)
* Secure API Access

## Real-Time Communication

* Socket.IO integration
* Real-time updates
* Live meeting interactions

## Organization Management

* Create organizations
* Join organizations
* Role-based access management

---

# System Architecture

```text
Frontend (React + Vite)
            │
            ▼
Backend (Node.js + Express)
            │
            ▼
MongoDB Database
            │
 ┌──────────┴──────────┐
 ▼                     ▼

Google Gemini      Pinecone

AI Summaries     Semantic Search
```

---

# Tech Stack

## Frontend

* React.js
* Vite
* Tailwind CSS
* React Router DOM
* Axios
* Recharts
* Chart.js
* Lucide React
* React Toastify
* React Speech Recognition
* Socket.IO Client

## Backend

* Node.js
* Express.js
* Socket.IO
* JWT Authentication
* Multer
* Nodemailer
* Cookie Parser
* CORS

## Database

* MongoDB
* Mongoose

## AI & Search

* Google Gemini API
* Pinecone
* Hugging Face Inference API
* ChromaDB
* Xenova Transformers
* ONNX Runtime
* OpenAI SDK (Optional)

## Integrations

* Google APIs
* Microsoft Graph API
* Calendar Utilities
* Email Services

---

# Project Structure

```text
MeetOnMemory
│
├── client
│   ├── public
│   ├── src
│   │   ├── assets
│   │   ├── components
│   │   ├── context
│   │   └── pages
│   └── package.json
│
├── server
│   ├── config
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── services
│   ├── socket
│   ├── uploads
│   ├── utils
│   └── server.js
│
├── package.json
└── README.md
```

---

# Screenshots

## Dashboard

![Dashboard](./screenshots/Dashboard.jpeg)

## Meeting Management

![Meeting Management](./screenshots/Meeting-management.jpeg)

## Reports & Analytics

![Analytics](./screenshots/Report-analytics.jpeg)

---

# Installation

## Clone Repository

```bash
git clone https://github.com/imuniqueshiv/MeetOnMemory.git

cd MeetOnMemory
```

---

## Backend Setup

```bash
cd server

npm install
```

Create `.env`

```env
PORT=4000

MONGODB_URI=your_mongodb_uri

JWT_SECRET=your_secret

NODE_ENV=development

SMTP_USER=your_email

SMTP_PASS=your_password

SENDER_EMAIL=your_email

ASSEMBLYAI_API_KEY=your_key

OPENAI_API_KEY=optional

HUGGINGFACE_API_KEY=your_key

GEMINI_API_KEY=your_key

GEMINI_MODEL=gemini-2.0-flash

PINECONE_API_KEY=your_key

PINECONE_ENVIRONMENT=your_environment

INDEX_NAME=your_index_name

TRANSFORMERS_BACKEND=onnxruntime-web
```

Start Backend:

```bash
npm run server
```

---

## Frontend Setup

```bash
cd client

npm install
```

Create `.env`

```env
VITE_BACKEND_URL=http://localhost:4000
```

Run Frontend:

```bash
npm run dev
```

---

# Environment Variables

### Server

| Variable             | Purpose               |
| -------------------- | --------------------- |
| PORT                 | Server Port           |
| MONGODB_URI          | MongoDB Connection    |
| JWT_SECRET           | Authentication Secret |
| GEMINI_API_KEY       | Google Gemini         |
| GEMINI_MODEL         | Gemini Model          |
| PINECONE_API_KEY     | Pinecone Access       |
| PINECONE_ENVIRONMENT | Pinecone Environment  |
| INDEX_NAME           | Pinecone Index        |
| HUGGINGFACE_API_KEY  | Embeddings            |
| ASSEMBLYAI_API_KEY   | Speech Processing     |
| SMTP_USER            | Email Service         |
| SMTP_PASS            | Email Service         |
| SENDER_EMAIL         | Sender Email          |

### Client

| Variable         | Purpose         |
| ---------------- | --------------- |
| VITE_BACKEND_URL | Backend API URL |

---

# Future Improvements

* Live Meeting Recording
* Real-Time Speech Transcription
* Voice Search
* Google Calendar Integration
* Outlook Integration
* AI Meeting Assistant
* Slack Integration
* Multi-Language Support
* Mobile Application

---

# Use Cases

### Organizations

Store and retrieve meeting knowledge efficiently.

### Educational Institutions

Manage meetings, events, and policy records.

### Research Teams

Maintain searchable archives of discussions and decisions.

### Startups

Track decisions, action items, and organizational growth.

---

# Contributors

### Shiv Raj Singh

B.Tech – Artificial Intelligence & Machine Learning

GitHub:
https://github.com/imuniqueshiv

LinkedIn:
https://www.linkedin.com/in/shiv-raj-singh-387973299/

---

# License

This project is licensed under the MIT License.

---

# Support

If you find this project useful:

⭐ Star the repository

🍴 Fork the project

🐛 Report issues

🤝 Contribute improvements

---

Built with React, Node.js, MongoDB, and AI.
