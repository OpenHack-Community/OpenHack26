# Smart Civic Complaint Triage System

## Team Name
AI Genesis

## Team Members
- Naeem Ahmed (Team Lead) — [@naeemz3260](https://github.com/naeemz3260)
- Ali Nawaz — [@alinawazcode](https://github.com/alinawazcode)
- Mohammad Mujtaba — [@MohammadMujtabasoomro](https://github.com/MohammadMujtabasoomro)

## Problem Statement
SC-01 — Improving civic accountability, accessibility, and the efficiency of everyday public services.

## Category
Category 5: Smart Communities & Public Services

## Solution
A transparent, explainable civic grievance reporting and municipal triage platform that addresses urban infrastructure decay across Pakistani municipalities (Karachi, Lahore, Khairpur).

Key capabilities:
- **Multilingual Citizen Ingestion:** Accepts grievance reports in English, Urdu script, and colloquial Roman Urdu (*"sarak toot gayi hai"*, *"gutter ubal raha hai"*).
- **Automated Duplicate Detection:** Uses geospatial Haversine distance ($\le 60\text{m}$) and 128-dimensional subword cosine text similarity ($\ge 0.75$) to cluster duplicate reports into unified municipal work orders and warn citizens before submission.
- **Explainable 4-Factor Priority Engine:** Calculates priority ($0\text{--}100$) based on Safety Risk, Unique Affected Population, SLA Age, and Local Recurrence, featuring an interactive What-If weight sandbox and guaranteed safety overrides for life hazards (bare live wires, open manholes).
- **Verified Field Closure:** Requires field workers to capture resolution proof via an in-app camera with baked municipal GPS/time watermarks, evaluated with Computer Vision blur/luminance checks and a Before/After comparison slider before supervisor sign-off.
- **Auditable Lifecycle & SLA Timers:** Full state machine with automated escalation alerts at 50%, 100% (overdue), and 150% (critical) SLA thresholds.

## Tech Stack
- **Frontend:** React 19, TypeScript, Vite, Tailwind CSS v4, Framer Motion, Lucide Icons, Recharts, i18next (with RTL Urdu support)
- **Maps & Telemetry:** Leaflet, React-Leaflet, CartoDB Open Tiles, HTML5 Geolocation API, HTML5 Canvas API
- **Backend Frameworks:** 
  - Python FastAPI (Pydantic v2, SQLAlchemy, Uvicorn)
  - Node.js / Express (TypeScript, REST API)
- **Database:** SQLite (Cross-platform zero-config embedded database with `sql.js` WASM and local disk persistence)
- **DevOps & Cloud:** Docker, Multi-stage Nginx builds, Railway Cloud deployment

## Challenges Faced
1. **Phonetic & Dialectal Roman Urdu NLP:** Standard NLP models fail on Roman Urdu due to non-standardized phonetic spelling (*"khadda"*, *"gadda"*, *"tooti road"*). We overcame this by designing a 128-dimensional subword character 3-gram embedding space mapped to municipal domain dictionaries.
2. **Preventing Ghost Resolutions:** Field staff often mark tickets resolved without genuine on-site work. We solved this with device-level camera streaming that stamps unforgeable canvas watermarks (live GPS coordinates, Pakistan Standard Time, ticket reference ID) and flags blurry images using Laplacian variance.
3. **Cross-Platform Zero-Config Portability:** Ensuring hackathon judges and evaluators can run the entire system locally without setting up external PostgreSQL or Docker databases. We implemented SQLite WASM disk persistence and unified client/server routing.
4. **Explainable AI vs. Black-Box Disconnect:** Instead of an uninterpretable neural network priority score, we built an explainable 4-factor scoring model that explicitly shows why a ticket is ranked high and allows municipal administrators to simulate weight changes in real-time.

## Learnings
- Learned how to fine-tune character n-gram text representations to bridge low-resource regional dialects (Roman Urdu) with semantic intent.
- Gained hands-on experience implementing spatio-temporal clustering algorithms that prevent municipal call centers from being paralyzed by redundant complaints.
- Mastered client-side Computer Vision techniques (Laplacian convolution kernels and luminance histograms) to assess photo quality in resource-constrained environments.
- Deepened understanding of role-based access control (RBAC) segregation between District Admins and Super Admins for sensitive municipal governance operations.

## AI / Open-Source Usage
- **NLP & Embeddings:** Scikit-Learn (TF-IDF vectorizers, Multiclass Logistic Regression) and 128-dimensional character 3-gram subword embeddings for English, Urdu, and Roman Urdu.
- **Computer Vision:** OpenCLIP zero-shot visual concepts, Pillow perceptual hash validation, and Laplacian edge kernel convolution for blur detection.
- **Mapping & Geodesic Tools:** OpenStreetMap, CartoDB tile layers, and mathematical Haversine geodesic distance algorithms.
- **Icons & UI:** Lucide React icons, Framer Motion animations, and Google Fonts (Inter, Noto Nastaliq Urdu).

## Project Repository
https://github.com/naeemz3260/Smart-Civic-Complaint-Triage-System
