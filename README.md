⸻

🚀 Magnus-Job-ApplyTrack

AI-Powered Job Application & Resume Intelligence Platform

A comprehensive platform that integrates job tracking, ATS-optimized resume analysis, and AI-driven job matching — designed for modern job seekers and recruiters.

⸻

🧠 Overview

Magnus-Job-ApplyTrack combines three key modules:

Module	Description
ApplyTrack	Tracks all job applications, status updates, and employer responses in one dashboard.
Talent Intelligence	Generates and optimizes ATS-compliant resumes and cover letters using AI.
AI-Match Engine	Suggests jobs based on profile, skills, and resume keywords using machine-learning matching.


⸻

🧩 Tech Stack

Frontend:
	•	⚛️ Next.js 14 (App Router)
	•	🎨 Tailwind CSS + TypeScript
	•	🧩 React Query + Axios

Backend:
	•	⚙️ FastAPI (Python 3.11)
	•	🗄️ PostgreSQL / Supabase
	•	🔁 Celery + Redis (background jobs)

DevOps / Infrastructure:
	•	☁️ Render / Vercel Deployment
	•	🐳 Docker Compose (backend + worker services)
	•	🧠 GitHub Actions (CI/CD)

⸻

📦 Repository Structure

Magnus-Job-ApplyTrack/
├── frontend/          # Next.js frontend
│   ├── app/           # App Router pages
│   ├── components/    # Reusable UI elements
│   └── lib/           # Helpers and utilities
├── backend/           # FastAPI backend (APIs & models)
├── mobile/            # React Native client (optional)
├── services/          # Shared modules (auth, utils)
├── App.tsx
├── index.html
├── types.ts
└── .gitignore


⸻

💡 Key Features

✅ AI Resume Builder – Create ATS-optimized resumes with dynamic keyword matching.
✅ Application Dashboard – Manage all job applications in one unified view.
✅ Job Matching Engine – Recommends roles based on profile analysis.
✅ Analytics Panel – Track application success rate, response trends, and performance metrics.
✅ Responsive UI – Designed for web + mobile viewing.

⸻

⚙️ Local Development

# 1️⃣ Clone repo
git clone https://github.com/chiosemen/Magnus-Job-ApplyTrack.git
cd Magnus-Job-ApplyTrack

# 2️⃣ Frontend
cd frontend
npm install
npm run dev

# 3️⃣ Backend (in another terminal)
cd ../backend
pip install -r requirements.txt
uvicorn app.main:app --reload


⸻

🧩 Environment Variables

Variable	Description
DATABASE_URL	PostgreSQL or Supabase database URL
REDIS_URL	Redis instance for Celery/queues
OPENAI_API_KEY	API key for AI resume analysis
SUPABASE_URL / SUPABASE_ANON_KEY	Auth & storage configuration
NEXT_PUBLIC_API_URL	Frontend → backend API endpoint


⸻

🧠 Architecture Diagram

flowchart TD
    A[User Interface<br>(Next.js Frontend)] --> B[API Gateway<br>(FastAPI Backend)]
    B --> C[PostgreSQL / Supabase DB]
    B --> D[Redis / Celery Workers]
    D -->|Async Tasks| E[AI Resume Processor]
    A -->|Fetch / POST| B


⸻

🚀 Deployment

Environment	Platform	Branch
Frontend	Vercel	main
Backend	Render	main
Database	Supabase	Persistent
CI/CD	GitHub Actions	Automated Deploy


⸻

🧑🏽‍💻 Author

Chinye Osemene (@chiosemen)
GitHub Profile | LinkedIn | Portfolio

⸻

🪄 License

MIT License © 2025 Chinye Osemene

⸻

