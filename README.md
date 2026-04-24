# 🚚 Enterprise Logistics System — Real-Time SaaS Platform

![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6)
![React](https://img.shields.io/badge/React-19-61DAFB)
![Cloudflare Workers](https://img.shields.io/badge/Edge-Cloudflare%20Workers-F38020)
![Real-Time](https://img.shields.io/badge/Real--Time-SSE-green)
![Automation](https://img.shields.io/badge/Automation-n8n%20%2B%20AI-purple)

Scalable logistics management system designed for real-world operations, featuring real-time tracking, routing optimization, and high data consistency.

> Built with a serverless edge architecture to support real-time operations, complex workflows, and production-grade reliability.

---

## 🧠 Problem

Logistics operations typically suffer from:

- Lack of real-time visibility across deliveries
- Manual routing and inefficient driver allocation
- Data inconsistency between operational steps
- No reliable audit trail for decision tracking

This platform was designed to solve these challenges using a real-time, event-driven architecture.

---

## 🏗️ Architecture Overview
Frontend (React SPA)
→ Cloudflare Edge (Workers + Hono)
→ D1 Database (SQLite)
→ Real-time layer (SSE)

### Key Decisions

- **Serverless architecture** for scalability and cost efficiency  
- **Edge computing (Cloudflare Workers)** for low-latency responses  
- **Server-Sent Events (SSE)** replacing polling  
- **State machine architecture** for order lifecycle control  
- **Event-driven audit system** for full traceability  

---

## ⚡ Key Features

### 📦 Order & Routing System
- Multi-driver routing with dynamic assignment
- Intelligent delivery allocation
- Route segmentation and optimization

### ⚙️ Workflow & Automation
- State-machine-based order lifecycle
- Automatic transitions based on system events
- Integration with automation pipelines (**n8n + Groq LLM**)

### 📡 Real-Time Infrastructure
- Live updates using SSE
- Instant notification system
- Real-time GPS tracking

### 📸 Validation System
- 3-step photo verification:
  - Pickup
  - Delivery
  - Proof-of-delivery (receipt)
- Automatic state transitions after validation

### 🚛 Fleet & Driver Management
- Vehicle maintenance tracking (KM-based alerts)
- Driver checklist system (EPI + vehicle condition)
- Fixed driver-vehicle assignment logic

### 🔐 Audit & Security
- Full event tracking system
- Operational traceability
- Role-based actions and validations

---

## 🚀 Impact

- **~97% reduction in API requests** (SSE vs polling)
- **Real-time updates < 1s latency**
- **High data consistency** via atomic operations
- **Production-ready architecture** for scaling logistics operations

---

## 🛠️ Tech Stack

### Frontend
- React
- TypeScript
- Tailwind CSS

### Backend
- Cloudflare Workers
- Hono (Edge API framework)

### Database
- D1 (SQLite - serverless)

### Real-Time
- Server-Sent Events (SSE)

### Automation & AI
- n8n (workflow automation)
- Groq LLM (AI-driven workflows)

### Architecture
- Serverless
- Edge Computing
- Event-driven design
- State machine orchestration

---

## 🧠 Engineering Highlights

- Atomic database operations to ensure consistency
- Optimistic locking to prevent race conditions
- Event-based audit system for full traceability
- Strict validation and state control across workflows
- Rate limiting and security middleware at the edge

---

## 📊 System Design Highlights

- Handles complex business rules (logistics + routing + validation)
- Designed for real-world operational workflows
- Modular architecture allowing future scaling (microservices ready)
- Separation of concerns between real-time, API, and persistence layers

---

## 🖼️ Demo

> ⚠️ Add screenshots and video demo here

Recommended:
- Dashboard
- Routing page
- Real-time tracking
- Driver app (checklist / photos)

---

## 🎯 Why This Project Matters

This system is not a prototype.

It is a **production-oriented platform** designed to handle:

- Real logistics operations
- High-frequency updates
- Complex business rules
- Real-time user interactions

---

## 📫 Contact

- GitHub: https://github.com/henriquebuilder  
- LinkedIn: https://www.linkedin.com/in/luis-henrique-da-silva-cunha-89bba8124  

---

## ⚠️ Disclaimer

This repository represents a **case study version** of a private commercial system.

Certain parts of the implementation — including sensitive business logic, integrations, and infrastructure details — have been intentionally omitted.

The purpose of this repository is to demonstrate **architecture decisions, system design, and engineering approach**.

---

## 📄 License

MIT
