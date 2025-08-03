
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

## 📦 Instalación manual

### 🔹 Frontend

```bash
cd frontend
npm install
npm run dev
```

### 🔹 Backend

```bash
cd backend

# Dependencias necesarias
npm install express cors dotenv

# Dependencia de desarrollo para autorecarga
npm install --save-dev nodemon
```

En `package.json`, asegúrate de tener:

```json
"type": "module",
"scripts": {
  "dev": "nodemon index.js"
}
```

---

## 🐳 Docker

Puedes levantar todo el proyecto con Docker:

### 🔧 1. Requisitos
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### ▶️ 2. Comando para levantar todo

```bash
docker-compose up --build
```

Esto construirá y levantará dos servicios:

- 🟦 **Frontend** (React + Vite): http://localhost:3000  
- 🟩 **Backend** (Node.js + Express): http://localhost:5000

---

## 🧾 Docker Structure

```
/frontend
  └── Dockerfile         ← builda React y sirve con Nginx

/backend
  └── Dockerfile         ← instala dependencias y lanza Express

/docker-compose.yml      ← orquesta ambos servicios
```

---

## 📝 .gitignore actualizado

Además del `.gitignore` raíz, cada subproyecto tiene su propio `.gitignore`:

### `/frontend/.gitignore`
```
node_modules/
.env
dist/
```

### `/backend/.gitignore`
```
node_modules/
.env
```

---

## 📁 Estructura inicial

```
/frontend     → React + Vite + Tailwind
/backend      → Node.js + Express + Mongo/PostgreSQL
/docs         → Prompts, diseños, notas
/scripts      → Seeders o migraciones
```

---

## 🧠 Funcionalidades clave

- Generación de rutinas con IA
- Feedback post-entreno según cómo te sientas
- Ocultación de pesos previos para evitar límites mentales
- Alternativas si una máquina está ocupada (con imágenes)
- Rutinas manuales para usuarios avanzados
- Soporte para tipos de agarre, dificultad, equipamiento
- Integración futura: nutrición, fotos, PDF, compartir progresos

---

## ✅ Roadmap del MVP

Ver el tablero en Trello para tareas activas.  
[Trello MVP Entrenamiento](#) *(añade el enlace al tablero aquí)*

---

## ✨ Autor

Creado con ❤️ por Rafa & ChatGPT
