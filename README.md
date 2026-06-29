# MindSpring AI - Frontend & Mobile Application 🧠💻📱

MindSpring AI is an AI-powered, adaptive tutoring platform tailored specifically for Pakistani Matric and Intermediate (BISE-style) students. This repository contains the complete user interface, adaptive learning dashboard, and mobile shell integration for the platform.

The application is built using **React 19** and **Vite 8** for a fast web experience, and wrapped with **Capacitor 7** to run as a native Android application.

---

## ✨ Core UI Pages & Features

- 📊 **Adaptive Dashboard:** Displays subject tiles, chapter progress bars, and performance analytics fetched from the backend.
- 📝 **Smart Notes Interface:** Custom layouts for generating and viewing AI-powered summaries, formulas, key points, and mindmaps.
- ⏱️ **Interactive MCQ Quiz:** Standalone quiz environment with timers, immediate evaluation, and dynamic difficulty scaling.
- 🗂️ **Active Recall Flashcards:** Flippable dynamic cards (`FlashcardTile`) for rapid revision.
- 🗓️ **Interactive Study Planner:** Displays AI-generated weekly/monthly schedules in beautiful colored block cards.
- 💬 **AI Tutor Chat:** Full chat interface featuring custom routing that connects to specific ingested textbooks.
- 📑 **PDF Summarizer UI:** Paste textbook content or upload `.txt`/`.md` files to instantly extract summaries and key questions.
- 🏛️ **Past Papers & Exam Tips:** Specific UI modules to generate past paper formats and exam preparation tips.
- 📚 **My Library:** A unified timeline where students can review saved notes, revisit past quiz attempts, or practice quiz batches again.
- 🖨️ **Client-Side PDF Export:** Fully responsive, off-screen A4 print sheets designed using `html2pdf.js` to let users download summaries, chat transcripts, study plans, and quizzes in print-ready layouts.

---

## 🛠️ Tech Stack

- **Core Framework:** React 19 (Component-based architecture and advanced state management)
- **Build Tool:** Vite 8 (Ultra-fast development server and production bundling)
- **Mobile Native Bridge:** Capacitor 7 (Wraps the web build into an Android project shell)
- **PDF Generation:** `html2pdf.js` (Pure client-side HTML-to-PDF compilation)

---

## 📂 Repository Structure

```text
frontend/
├── src/
│   ├── App.jsx             # Main application orchestrator (Pages, state, & layout)
│   ├── Signup.jsx          # Custom Auth UI (Login/Signup connected to Flask API)
│   ├── adaptiveSync.js     # Centralized backend HTTP client helpers
│   ├── apiConfig.js        # API Base configuration handler
│   ├── PdfExport.jsx       # Print-friendly layout components (A4 sheets)
│   ├── pdfExport.js        # Core html2pdf wrapper utility
│   ├── Quiz.jsx            # Alternate/auxiliary quiz engine
│   └── main.jsx            # React application entry point
├── .env.local              # Local environment overrides
├── .env.example            # Environment variables blueprint
├── capacitor.config.json   # Capacitor bridge configurations
└── android/                # Native Android studio project files
