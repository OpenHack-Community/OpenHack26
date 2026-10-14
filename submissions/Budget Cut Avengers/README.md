# CivicSense 🏙️✨
### Smart Civic Complaint Triage & Resolution Ecosystem

## Team Name
Budget Cut Avengers

## Team Members
- Mahnoor Atta (Team Lead) — @Mahnoor-atta
- Maham Ali Lodhi — @lodhimahamali
- Syeda Soofia Shah — @Soofiashah

## Problem Statement
**Problem SC-01 — Smart Civic Complaint Triage System** 
*(Bridging the gap between citizens and municipal authorities through transparent reporting, automated triage, and workflow automation.)*

## Category
Smart Communities & Public Services

## 🚀 Executive Summary / Solution
**CivicSense** is an enterprise-grade, minimalist civic grievance platform engineered to eradicate administrative bottlenecks. Unlike traditional clunky portals, CivicSense features:
1. **AI-Powered Automated Triage:** Leverages **Google Gemini AI** to instantly parse citizen text descriptions, auto-categorize issues, and assign severity priorities.
2. **Smart Duplicate Detection Engine:** Intelligently identifies and flags recurring or duplicate complaints within the same area, preventing administrative redundancy.
3. **Multi-Tier Role-Based Workflow:** A seamless lifecycle management system flowing from *Citizens (Reporters)* -> *Admins (Triage & Forward)* -> *Higher Authority/Faculty (Resolution & Evidence)*.

## 🛠️ Tech Stack & Architecture
- **Frontend:** React.js (Vite), Tailwind CSS (Aesthetic soft pastel minimalist theme with custom micro-interactions)
- **Backend & Database:** Firebase Firestore (Real-time data synchronization & optimized Base64 media storage layer)
- **Intelligence Layer:** Google Gemini API (Structured automated text analysis and severity scoring)
- **Deployment & Scaling:** Vercel (Production-ready secure environment variables architecture)

## 🔥 Core Features Implemented (Meeting Expected MVP)
- [x] **Multi-Modal Submissions:** Clean citizen portal supporting text, photographic evidence, and precise location mapping.
- [x] **AI Classification & Triage:** Automated categorization and priority assignment powered by Gemini.
- [x] **Duplicate Prevention:** Algorithmic detection of potential duplicate reports to keep municipal queues clean.
- [x] **Configurable Action Rules:** Admin review panel equipped with deadline allocators and rejection/forwarding pathways.
- [x] **Transparent Status Tracking:** Real-time updates from *Pending ➔ Forwarded ➔ Resolved* with full audit trails.

## 🚧 Challenges Faced & Overcome
- **CORS & Storage Optimization:** Bypassed strict free-tier storage restrictions by engineering an optimized Base64-to-Firestore streaming pipeline, ensuring zero-latency image rendering across dashboards.
- **Role-Based State Management:** Architected a secure, multi-tier login routing system (`noor`, `admin`, `faculty` test handles) ensuring strict boundary lines between citizen reporting and administrative controls.

## 💡 Key Learnings
- Mastered the integration of generative AI (Gemini SDK) for real-world municipal workflow automation.
- Gained deep expertise in scalable React state management and secure cloud environment variable handling.

## 🤖 AI & Open-Source Usage Disclosure
- **Google AI Studio (Gemini Flash):** Utilized for backend text parsing, categorization logic, and triage intelligence.
- **Tailwind CSS & Open-Source Libraries:** Utilized for rapid, accessible, and high-performance UI components.

## 📂 Project Repository & Live Demo
- **Live Production URL:** [https://civic-sense-complaints.vercel.app](https://civic-sense-complaints.vercel.app)
- **GitHub Code Repository:** https://github.com/Mahnoor-atta/CivicSense
