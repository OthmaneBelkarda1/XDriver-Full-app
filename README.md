# 🚗 XDriver — Smart Carpooling Platform

XDriver is a full-stack carpooling application that connects drivers and passengers with AI-powered pricing, a modern React frontend, and a robust Django backend.

---

## 🏗️ Architecture Overview

```
┌─────────────────┐     ┌─────────────────┐     ┌──────────────────────┐
│   React Frontend │────▶│  Django Backend  │────▶│  ML Price Prediction │
│    (Lovable)     │     │   (REST API)     │     │  (scikit-learn +     │
└─────────────────┘     └─────────────────┘     │      FastAPI)        │
                                │                └──────────────────────┘
                                ▼
                        ┌─────────────────┐
                        │   MCP Server    │
                        │    (Python)     │
                        └─────────────────┘
```

---

## 📦 Repositories

| Component | Tech Stack | Repository |
|-----------|-----------|------------|
| 🖥️ **Frontend** | React (Lovable) | [rideshare-connect](https://github.com/OthmaneBelkarda1/rideshare-connect) |
| ⚙️ **Backend** | Django, REST API | [Xdriver](https://github.com/OthmaneBelkarda1/Xdriver) |
| 🤖 **ML Price Model** | scikit-learn, FastAPI | [carpooling-price-prediction](https://github.com/OthmaneBelkarda1/carpooling-price-prediction) |
| 🔌 **MCP Server** | Python | [Carpooling_MCP_SERVER](https://github.com/OthmaneBelkarda1/Carpooling_MCP_SERVER) |

---

## ✨ Features

- 🗺️ **Ride Matching** — Connect drivers and passengers going the same route
- 💰 **AI-Powered Pricing** — ML model predicts fair ride prices based on distance, demand, and other factors
- 🔐 **User Authentication** — Secure login and profile management via Django backend
- 🤖 **MCP Server** — Model Context Protocol server for AI assistant integrations
- 📱 **Responsive UI** — Modern React frontend built with Lovable

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- Python (3.10+)
- pip / pipenv

### 1. Clone all repositories

```bash
git clone https://github.com/OthmaneBelkarda1/rideshare-connect       # Frontend
git clone https://github.com/OthmaneBelkarda1/Xdriver                  # Backend
git clone https://github.com/OthmaneBelkarda1/carpooling-price-prediction  # ML API
git clone https://github.com/OthmaneBelkarda1/Carpooling_MCP_SERVER    # MCP Server
```

### 2. Run the Backend

```bash
cd Xdriver
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### 3. Run the ML Price API

```bash
cd carpooling-price-prediction
pip install -r requirements.txt
uvicorn main:app --reload --port 8001
```

### 4. Run the Frontend

```bash
cd rideshare-connect
npm install
npm run dev
```

### 5. Run the MCP Server

```bash
cd Carpooling_MCP_SERVER
pip install -r requirements.txt
python server.py
```

---

## 🧠 ML Price Model

The price prediction model is trained with **scikit-learn** and served via **FastAPI**. It takes inputs such as:
- Trip distance
- Time of day
- Number of passengers
- Route popularity

And returns a suggested fare for the ride.

---

## 🔌 MCP Server

The MCP (Model Context Protocol) server allows AI assistants (like Claude) to interact with the XDriver platform — querying rides, managing bookings, and more through natural language.

---

## 👤 Author

**Othmane Belkarda**
- GitHub: [@OthmaneBelkarda1](https://github.com/OthmaneBelkarda1)

---

## 📄 License

This project is open source. See individual repositories for license details.
