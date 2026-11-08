# AURA - AI-Powered Therapy & Mental Health Platform

**AURA** is an intelligent, scalable mental health and therapy platform designed to provide personalized psychological support, real-time emotion tracking, and AI-assisted conversational guidance. Built using modern architecture, AURA combines a **React** frontend, a high-performance **FastAPI** backend, and specialized **AI/ML pipelines**.

---

## 🌟 Key Features & Modules

- **🤖 Conversational AI Therapist:** Real-time conversational interface providing empathetic and structured support using fine-tuned LLMs & external APIs.
- **🧠 Emotion & Sentiment Analysis:** Natural Language Processing (NLP) models to evaluate user mood, stress levels, and emotional trends from chat logs.
- **📚 RAG Engine (Knowledge Base):** Retrieval-Augmented Generation system connected to verified psychological resources for evidence-based responses.
- **📊 User Mental Health Dashboard:** Visual insight panels tracking therapeutic progression, mood history, and actionable recommendations.

---

## 🏗 System Architecture

```text
┌─────────────────────────────────────────────────────────────┐
│                       AURA Architecture                      │
└─────────────────────────────────────────────────────────────┘
                               │
            ┌──────────────────┴──────────────────┐
            ▼                                     ▼
     ┌──────────────┐                      ┌──────────────┐
     │  React Web   │                      │  Mobile App  │
     │  (Frontend)  │                      │   (Future)   │
     └──────┬───────┘                      └──────┬───────┘
            │                                     │
            └──────────────────┬──────────────────┘
                               │ HTTP / WebSockets
                               ▼
                    ┌─────────────────────┐
                    │   FastAPI Backend   │
                    └──────────┬──────────┘
                               │
    ┌──────────────────────────┼──────────────────────────┐
    ▼                          ▼                          ▼
┌──────────────┐       ┌──────────────┐       ┌──────────────┐
│  AI Engine   │       │ RAG Pipeline │       │ PostgreSQL   │
│ & Fine-Tuned │       │ & Vector DB  │       │  Database    │
│    Models    │       │ (LangChain)  │       │              │
└──────────────┘       └──────────────┘       └──────────────┘
```
📂 Repository Structure

AURA-AI-Therapy/
├── frontend/             # React application (UI Components, State Management)
├── backend/              # FastAPI application (REST Endpoints, Auth, DB Models)
├── ai_models/            # AI pipelines (Fine-tuning scripts, RAG setup, APIs)
└── docs/                 # Documentation & UI/UX Design assets

--------------------------------------------------------------------------------

🛠 Tech Stack

- Frontend: React.js, TailwindCSS, Axios
- Backend: Python 3.10+, FastAPI, Pydantic, SQLAlchemy
- Database & Storage: PostgreSQL, Redis, Qdrant / ChromaDB (Vector DB)
- AI / ML Frameworks: PyTorch, HuggingFace Transformers, LangChain, OpenAI APIs

--------------------------------------------------------------------------------

🚀 Getting Started (Local Development)

### Prerequisites
- Python 3.10+
- Node.js 18+ & npm

### Backend Setup
1. Navigate to backend directory:
   cd backend

2. Create and activate a virtual environment:
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies:
   pip install -r requirements.txt

4. Copy the environment variables:
   cp .env.example .env

5. Run the server:
   uvicorn app.main:app --reload

### Frontend Setup
1. Navigate to frontend directory:
   cd frontend

2. Install packages:
   npm install

3. Start development server:
   npm start

--------------------------------------------------------------------------------

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
