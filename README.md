# 🌿 AyurCare: Smart Panchakarma Solution for Community Health

> **A digital healthcare platform designed to bridge the gap between ancient Ayurvedic healing and modern AI technology, improving patient adherence and therapy outcomes for community wellness centers.**

Proudly developed as a community health initiative, with applications suited for NGOs like **The Earth Saviours Foundation**, to streamline Panchakarma therapy management for marginalized and elderly patients.

---

## ✨ Core Features

### 🤖 AI Microservices Suite (Python/FastAPI)
* **AI Dosha Predictor:** Real-time algorithmic analysis calculating Vata, Pitta, and Kapha dominance based on physical and behavioral inputs.
* **Therapy Recommendation Engine:** Automatically maps the predicted Dosha to traditional Panchakarma treatments.
* **Ayurveda AI Chatbot:** Floating NLP widget to answer patient queries about therapies and wellness.
* **Sentiment Analysis:** Analyzes post-therapy patient feedback to flag negative/warning trends to practitioners.

### 👤 Patient Portal
* **Therapy Booking:** Interactive calendar to book sessions (Vamana, Virechana, etc.) in IST.
* **Pre-Procedure Guidance:** Checklists for therapy preparation (e.g., diet restrictions, exercise limits).
* **Recovery Progress Analyzer:** Daily logging of Energy, Sleep, and Pain levels, visualized on interactive `Recharts` graphs.
* **Emergency Helpdesk:** Direct SOS buttons for Indian National Emergencies (112, 108) and NGO helplines.

### 👨‍⚕️ Practitioner Dashboard
* **Clinical Records:** View assigned patients and their AI Dosha profiles.
* **Therapy Notes:** Add and securely save clinical observation notes.
* **Feedback Monitoring:** Instantly run AI Sentiment Analysis on patient reviews to monitor treatment efficacy.

### 📊 Admin & NGO Impact Dashboard
* **Community Command Center:** High-level metrics for total patients, active therapies, and success rates.
* **NGO Impact Metrics:** Track free therapies sponsored, rural participation, and total people served.
* **Therapy Management:** Master catalog to edit therapy durations, pre-guidelines, and post-recovery steps.

---

## 🛠️ Technology Stack

**Frontend:**
* React.js (Vite)
* Tailwind CSS (Styling & UI)
* Lucide React (Icons)
* Recharts (Data Visualization)
* React Router (Navigation)

**Backend:**
* Node.js & Express.js
* MongoDB & Mongoose (Database)
* JSON Web Tokens (JWT) for Role-Based Authentication

**AI Microservice:**
* Python 3
* FastAPI & Uvicorn

---

## 🚀 How to Run Locally

To evaluate or develop this project locally, you will need to run three separate terminal instances.

### 1. Start the Node.js Backend
```bash
cd backend
npm install
# Ensure you have your MongoDB URI and JWT_SECRET in a .env file
node server.js

```
Runs on http://localhost:5000 

### 2. Start the Python AI Microservice
```bash
cd ai-service
pip install fastapi uvicorn pydantic
uvicorn main:app --reload --port 8000
```
Runs on http://localhost:5000 

### 3. Start the React Frontend
```bash
cd frontend
npm install
npm install recharts lucide-react react-router-dom
npm run dev
```
Runs on http://localhost:5173





