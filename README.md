# 🚗 XDriver — Smart Carpooling Platform

XDriver is a full-stack carpooling application that connects drivers and passengers with AI-powered pricing — allowing passengers to search and book rides directly from WhatsApp, through a modern React frontend, and a robust Django backend.

---

## 🏗️ Architecture Overview

```
┌─────────────────┐     ┌─────────────────┐     ┌──────────────────────┐
│   React Frontend│───▶│  Django Backend│───▶│  ML Price Prediction │
│    (Lovable)    │     │   (REST API)    │     │  (scikit-learn +     │
└─────────────────┘     └─────────────────┘     │     FastAPI)         │
                                │               └──────────────────────┘
                                ▼
                        ┌─────────────────┐
                        │   MCP Server    │
                        │    (Node.js)    │
                        └─────────────────┘
```

---

## 📦 Repositories

| Component | Tech Stack | Repository |
|-----------|-----------|------------|
| 🖥️ **Frontend** | React (Lovable) | [Xdriver FrontEnd][https://github.com/OthmaneBelkarda1/xdriver-FrontEnd) |
| ⚙️ **Backend** | Django| [Xdriver Back end](https://github.com/OthmaneBelkarda1/Xdriver) |
| 🤖 **ML Price Model** | scikit-learn, FastAPI | [carpooling-price-prediction](https://github.com/OthmaneBelkarda1/carpooling-price-prediction) |
| 🔌 **MCP Server** | Node.js | [Carpooling_MCP_SERVER](https://github.com/OthmaneBelkarda1/Carpooling_MCP_SERVER) |

---

## ✨ Features

- 🗺️ **Ride Matching** — Connect drivers and passengers going the same route
- 💰 **AI-Powered Pricing** — ML model predicts fair ride prices based on distance, demand, and other factors
- 🤖 **MCP Server** — Model Context Protocol server for AI assistant integrations
- 📱 **Responsive UI** — Modern React frontend built with Lovable

---

## 🧠 ML Price Model

The price prediction model is trained with **scikit-learn** and served via **FastAPI**. It takes inputs such as:
- Trip distance
- Time of day
- Number of passengers

And returns a suggested price for the ride.

---

## 🔌 MCP Server

The MCP (Model Context Protocol) server allows AI assistants (like a WhatsApp ChatBot) to interact with the XDriver platform — searching for rides and booking them.

---

## 👤 Author

**Othmane Belkarda**
- GitHub: [@OthmaneBelkarda1](https://github.com/OthmaneBelkarda1)

---

## 📄 License

This project is open source. See individual repositories for license details.
