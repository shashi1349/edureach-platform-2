# 🎓 EduReach — Agentic College Chatbot

AI In The Real World — Connecting Students with Institutions

EduReach is a full-stack AI-powered platform that helps students instantly access accurate college information through an intelligent chatbot and AI voice counselor.

---

## 🚀 Problem

Students struggle to find basic information on college websites:

- 🔍 Too many pages → hard to find specific details  
- 📞 Limited office hours → delayed responses  
- 📧 Email delays → slow communication  
- 🏫 Physical visits → time-consuming  

---

## 💡 Solution

EduReach provides:

- 🤖 Agentic RAG Chatbot
  - Searches a custom college knowledge base
  - Uses AI (Google Gemini) for accurate answers
  - Tool-calling based intelligent retrieval

- 📞 AI Voice Counselor (Ava)
  - Makes real phone calls to students
  - Provides conversational guidance

- 🌐 Modern Web Platform
  - Clean UI with course, mentor & placement info
  - Gated content for logged-in users

- 🔐 JWT Authentication
  - Secure login/signup system
  - Controls access to premium features

---

## 🧠 Key Features

| Feature | Visitor | Logged-in User |
|--------|--------|---------------|
| Homepage (above mentors) | ✅ | ✅ |
| Full content | ❌ | ✅ |
| AI Chatbot | ❌ | ✅ |
| AI Voice Call | ❌ | ✅ |
| Signup Popup | ✅ | ❌ |

---

## 🏗️ Tech Stack

### Frontend
- React + TypeScript (Vite)
- Tailwind CSS
- Axios
- React Router

### Backend
- Node.js (v24)
- Express.js
- TypeScript
- MongoDB Atlas
- Mongoose

### AI & Tools
- Google Gemini (LLM + Embeddings)
- LangChain
- MongoDB Vector Search
- Vapi (Voice AI)

---

## 📁 Project Structure

edureach-platform/ 

├── client/                # React frontend 

├── server/                # Node backend

│   ├── src/ 

│   ├── knowledge-base/ 

│   └── dist/

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

bash git clone https://github.com/shashi1349/edureach-platform-2 

---

### 2️⃣ Backend Setup

bash cd server npm install 

Create .env file:

env PORT=5000 MONGODB_URI=your_mongodb_uri JWT_SECRET=your_secret JWT_EXPIRES_IN=7d CLIENT_URL=http://localhost:5173 GOOGLE_API_KEY=your_gemini_key  # Optional (Voice AI) VAPI_API_KEY=your_key VAPI_ASSISTANT_ID=your_id VAPI_PHONE_NUMBER_ID=your_id 

Run backend:

bash npm run dev 

---

### 3️⃣ Frontend Setup

bash cd client npm install npm run dev 

---

## 🤖 AI Architecture (RAG)

### Flow:

User Question ->
Vector Search (MongoDB Atlas) ->
Relevant Knowledge Chunks ->
Gemini LLM ->
Accurate Response


---

## 📡 API Endpoints

### Auth
- POST /api/auth/register
- POST /api/auth/login
- GET /api/auth/me

### Chat
- POST /api/chat/message

### Voice
- POST /api/vapi/call

---

## 🧪 Example API Request

json POST /api/chat/message {   "message": "What is the fee for B.Tech CSE?" } 

### Response

json {   "success": true,   "data": {     "response": "The B.Tech CSE tuition fee is ₹1,50,000 per year..."   } } 

---

## 🌍 Real-World Inspiration

- Duolingo → AI conversation learning  
- Ivy.ai → University chatbots  
- Bland.ai → Voice agents  
- Intercom Fin → RAG-based support  

---

## 🔥 What Makes EduReach Unique

- Combines Chat AI + Voice AI
- Uses Agentic RAG (not basic RAG)
- Fully production-ready architecture
- Real-world college use case

---

## 🚀 Deployment

### Backend (Render)

- Root Directory: server
- Build Command:
  bash   npm install && npm run build   
- Start Command:
  bash   npm start   

### Frontend (Vercel / Netlify)

- Build:
  bash   npm run build   

---

## 📌 Future Improvements

- Multi-college support  
- Admin dashboard  
- Analytics for student queries  
- Multi-language chatbot  

---

## Link to application : 

  https://edureach-platform-2.vercel.app/

---
## 👨‍💻 Author

P Shashikiran Reddy
B.Tech CSE Student  
