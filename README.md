# 🏋️‍♂️ Smart Gym App

**Entrena según cómo te sientes, no solo por los números.**  
Esta app revoluciona el seguimiento del gimnasio: combina React, Node.js, Mongo/PostgreSQL y OpenAI para ayudarte a entrenar de forma inteligente, humana y visual.

---

## 🚀 Tecnologías

### Frontend
- React (con Vite)
- TailwindCSS
- OpenAI integration (entrenador virtual)
- Responsive UI + Experiencia mobile-first

### Backend
- Node.js + Express
- MongoDB o PostgreSQL
- JWT Authentication
- REST API
- GPT endpoints

---

---

## ⚙️ Pasos para instalar todo

### 1. 🔧 Backend: Node + Express

```bash
mkdir backend && cd backend
npm init -y
npm install express cors dotenv
npm install --save-dev nodemon

# Crear archivo base
touch index.js
mkdir routes controllers models
