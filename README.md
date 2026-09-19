# 🌱 AI Enterprise Sustainability Agent

> An intelligent, full-stack AI agent that helps enterprises measure carbon emissions, 
> track ESG metrics, predict environmental impact with machine learning, and receive 
> AI-driven sustainability recommendations — all in real time.

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Python](https://img.shields.io/badge/python-3.10+-blue)
![React](https://img.shields.io/badge/react-18-61dafb)
![FastAPI](https://img.shields.io/badge/FastAPI-0.110-009688)
![License](https://img.shields.io/badge/license-MIT-green)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)

---

## 📖 Overview

**AI Enterprise Sustainability Agent** is a full-stack platform designed to simulate how modern 
enterprises monitor, analyze, and reduce their environmental footprint. It combines **real-time 
IoT data simulation**, **CPU-optimized machine learning models**, **Google Gemini AI 
recommendations**, and a **beautiful React dashboard** to give businesses a 360° view of their 
sustainability performance.

This project is built as a **practice / portfolio project** — no GPU required, runs on any 
normal laptop. Perfect for demonstrating full-stack + AI + ML skills.

---

## ✨ Key Features

### 🌍 1. Carbon Emission Measurement
- Track emissions from electricity, transportation, manufacturing, and waste
- Automatic CO₂e calculation using standardized emission factors
- Source-wise breakdown with historical trends

### 📊 2. ESG Metric Tracking
- Environmental, Social, and Governance scores
- Custom KPI dashboard with real-time updates
- Trend analysis and benchmarking

### 🔮 3. Environmental Impact Prediction
- CPU-optimized ML models (Linear Regression, Random Forest, Time Series)
- Forecast future emissions based on historical data
- Scenario simulation (what-if analysis)

### 🤖 4. AI-Powered Recommendations (Gemini)
- Google Gemini API integration
- Context-aware sustainability suggestions
- Actionable initiatives with priority ranking

### 📡 5. Real-Time IoT Simulation
- Simulated smart sensors (energy meters, air quality, water usage)
- Live data streaming to dashboard
- Background scheduler with APScheduler

### 📈 6. Interactive Dashboard
- Beautiful React + Tailwind UI
- Recharts-powered visualizations
- Role-based access (Admin / Analyst / Viewer)

### 🔐 7. Authentication & Security
- JWT-based authentication
- Password hashing with bcrypt
- Rate limiting and audit logs

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|--------------|
| **Frontend** | React 18, Vite, TailwindCSS, shadcn/ui, Recharts, Axios, React Router |
| **Backend** | FastAPI, SQLAlchemy, Pydantic, JWT, Alembic, APScheduler |
| **ML/Analytics** | scikit-learn, pandas, numpy, joblib |
| **AI** | Google Gemini API (`google-generativeai`) |
| **Database** | SQLite (dev) / PostgreSQL (optional) |
| **IoT** | Python-based device simulator |
| **DevOps** | Docker, GitHub Actions |

---

## 🏗️ Architecture



---

## 🚀 Quick Start

### Prerequisites
- **Python** 3.10+
- **Node.js** 18+
- **Git**
- **Gemini API key** → [Get it here (free)](https://aistudio.google.com/app/apikey)

---

### 🔧 Backend Setup

```bash
# 1. Navigate to backend
cd backend

# 2. Create virtual environment
python -m venv venv

# 3. Activate it
# Windows:
venv\Scripts\activate
# macOS / Linux:
source venv/bin/activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Setup environment variables
copy .env.example .env       # Windows
cp .env.example .env         # Mac/Linux

# 6. Add your Gemini API key inside .env
# GEMINI_API_KEY=your_api_key_here

# 7. Initialize database & seed data
python scripts/seed_data.py

# 8. Run the server
uvicorn main:app --reload\

# 1. Navigate to frontend
cd frontend

# 2. Install dependencies
npm install

# 3. Setup env
copy .env.example .env       # Windows
cp .env.example .env         # Mac/Linux

# 4. Run dev server
npm run dev