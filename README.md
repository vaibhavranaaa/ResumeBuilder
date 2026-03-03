# 📄 ResumeBuilder — Full Stack Resume Creation Platform

A modern, full-stack resume builder that lets users create, edit, preview, and export professional resumes through a guided multi-step workflow. Built with **React + Vite** on the frontend and **Spring Boot + MongoDB** on the backend.

---

## 📁 Project Structure

```
ResumeBuilder/
├── frontend/
│   └── resume-builder/            # React + Vite client
└── backend/
    └── resumebuilderapi/
        └── resumebuilderapi/      # Spring Boot API
```

---

## 🛠️ Tech Stack

| Layer | Tech |
|---|---|
| Frontend | React, Vite, React Router, Tailwind CSS, Axios |
| Export | jsPDF, html2canvas |
| Backend | Java 21, Spring Boot, Spring Data MongoDB, Spring Security |
| Auth | JWT |
| Integrations | Cloudinary (image storage), Razorpay (payments) |
| Build Tools | Maven, npm |

---

## ✨ Features

### 🧑‍💻 Frontend (`frontend/resume-builder`)
- Responsive landing page with login/register entry points
- User dashboard for creating and managing multiple resumes
- Multi-step resume editor covering:
  - Profile & contact info
  - Education and work experience
  - Skills, projects, and certifications
  - Additional information
- Resume template selection with live preview
- PDF and image export via jsPDF + html2canvas
- Razorpay payment flow integration scaffold

### ⚙️ Backend (`backend/resumebuilderapi`)
- Spring Boot REST API foundation
- MongoDB integration via Spring Data
- JWT-based authentication setup
- Bean validation for request handling
- Mail service integration
- Cloudinary SDK for image uploads
- Razorpay Java SDK for payment processing

> **Note:** Backend source implementation is partially scaffolded in this snapshot. All dependencies and project configuration are fully defined and ready for development.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd ResumeBuilder
```

### 2. Start the Frontend

```bash
cd frontend/resume-builder
npm install
npm run dev
```

Frontend dev server: `http://localhost:5173`

### 3. Start the Backend

**macOS / Linux:**
```bash
cd backend/resumebuilderapi/resumebuilderapi
./mvnw spring-boot:run
```

**Windows:**
```bash
cd backend\resumebuilderapi\resumebuilderapi
mvnw.cmd spring-boot:run
```

Backend API: `http://localhost:8080`

---

## 🔗 API Connectivity

The frontend is pre-configured to point to `http://localhost:8080` as the API base URL.

If your backend runs on a different host or port, update the base URL in:

```
frontend/resume-builder/src/utils/apiPaths.js
```

---

## 📜 Frontend Scripts

Run these from `frontend/resume-builder/`:

```bash
npm run dev       # Start development server
npm run build     # Production build
npm run preview   # Preview production build locally
npm run lint      # Run ESLint
```

---

## 🗺️ Roadmap / Suggested Improvements

- [ ] Add a root-level `.env.example` with all required environment variable keys
- [ ] Add `application.yml` example for MongoDB URI, JWT secret, mail, Cloudinary, and Razorpay config
- [ ] Add OpenAPI / Swagger documentation for backend endpoints
- [ ] Add unit and integration tests for both frontend and backend
- [ ] Complete backend source implementation for all API endpoints
- [ ] Add resume version history and autosave

---

## 📄 License

This project does not currently include a license. If you plan to distribute or open-source it, consider adding a `LICENSE` file. See [choosealicense.com](https://choosealicense.com) for guidance.

---

> Built with ☕ Java, ⚛️ React, and a passion for clean, professional resumes.
