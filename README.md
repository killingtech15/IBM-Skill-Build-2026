Digital Thriving Hub

A Full-Stack Digital Wellbeing & Cybersecurity Platform

Founders:
Shaik Muhammed Muzakir
Mohammed Muabbir Sayeed


---

Overview

Digital Thriving Hub is a mobile-first, full-stack Progressive Web Application (PWA) designed to help individuals transition from compulsive digital consumption to structured, productive, and secure digital behavior.

The MVP integrates:

Focus & productivity tracking

ML-based relapse prediction

Digital Hygiene Score (transparent formula)

Cybersecurity complaint submission (government routing integration)

Student utility services (jobs, weather)

Institutional analytics dashboard (server-side PDF reports)


This is not a blocking tool.
It is a behavioral governance system.


---

Problem Statement

Modern students struggle with:

Compulsive scrolling

Lack of sustained focus

Poor digital self-regulation

Increasing exposure to cybercrime

Fragmented productivity tools


Existing solutions solve isolated problems. Digital Thriving Hub unifies behavioral correction, cybersecurity workflow, and analytics in one ecosystem.


---

MVP Scope

Included

JWT-based authentication (Access + Refresh tokens)

Pomodoro focus tracking system

Time-series relapse prediction (ML microservice)

Transparent Digital Hygiene Score

Cyber complaint submission workflow

Weather & job utilities

Admin analytics dashboard

Server-side PDF report generation

English-only interface


Excluded (Planned for V2)

Community layer

Multi-language support

End-to-end encryption

Multi-tenant SaaS architecture



---

Tech Stack

Frontend

Next.js (React)

Tailwind CSS

Progressive Web App (PWA)

Service Workers


Backend

Node.js

Express

MongoDB Atlas

JWT Authentication

Role-based Middleware


Machine Learning Layer

Python (FastAPI)

Time-Series Relapse Prediction Model (LSTM/Temporal Model)


Optional Integrations

Redis (Caching)

Firebase (Push Notifications)

Cloudinary (File Uploads)


Deployment

Frontend: Vercel

Backend: Render

Database: MongoDB Atlas



---

System Architecture

Client (PWA)
→ Node.js API
→ MongoDB Database
→ ML Microservice (Relapse Prediction)
→ Government Cybercrime Portal Integration

Layered Architecture:

1. Presentation Layer (Frontend)


2. Application Layer (Node/Express)


3. Behavioral Intelligence Layer (ML Service)


4. Data Layer (MongoDB)


5. Integration Layer (Government routing)




---

Digital Hygiene Score (Transparent Formula)

Score =
(0.4 × Weekly Focus Consistency Index) +
(0.3 × Streak Stability Ratio) +
(0.2 × Mood Stability Index) −
(0.1 × Relapse Frequency Index)

All metrics normalized to 0–100 scale.

No black-box scoring.


---

ML-Based Relapse Prediction

Objective: Predict probability of user relapse (48+ hours without structured focus session).

Features Used:

Daily focus duration

Time gaps between sessions

Mood variability

Streak breaks

Session completion ratio


Model Flow:

1. Collect time-series behavioral data


2. Train temporal model (LSTM or equivalent)


3. Output relapse probability (0–1)


4. Trigger adaptive intervention if threshold exceeded



This system predicts patterns — it does not surveil behavior.


---

Cybersecurity Complaint Workflow

1. User submits complaint


2. Unique ID generated


3. Internal validation


4. Structured complaint packet prepared


5. Routed to official government cybercrime portal


6. Government reference ID stored


7. User notified



The platform acts as a facilitator, not an investigative authority.


---

API Structure (MVP)

Auth

POST /api/auth/register
POST /api/auth/login
POST /api/auth/refresh

Focus

POST /api/focus/start
POST /api/focus/end
GET /api/focus/stats

Complaints

POST /api/complaints
GET /api/complaints/user

Admin

GET /api/admin/analytics
GET /api/admin/reports


---

Security Architecture

bcrypt password hashing

JWT expiration policies

Refresh token rotation

HTTPS enforcement

Input validation (Joi)

Rate limiting

File upload size restriction (5MB)

Data export & account deletion support


Advanced encryption planned for V2.


---

Offline-First Capabilities

Service Worker Caches:

Static assets

Dashboard snapshot

Saved jobs

Complaint drafts


IndexedDB Stores:

Draft complaints

Notes


Background sync restores data when online.


---

Institutional Dashboard

Admin Metrics:

Average focus hours

Relapse prediction distribution

Complaint category breakdown

Resolution time analytics

Active users


Reports generated server-side (PDF export).


---

Performance Targets

API response time < 500ms

Lazy-loaded routes

CDN-backed static assets

Image upload limit: 5MB



---

Roadmap

V2:

Multi-language support

Field-level encryption

Community layer

Multi-tenant SaaS model

Advanced adaptive friction personalization

Behavioral clustering analytics



---

Philosophy

Digital Thriving Hub does not enforce restriction.

It provides structured scaffolding until discipline becomes internal.

The long-term goal is user independence.


---

License

To be defined (MIT / Proprietary / Hybrid)


---

Contributing

MVP currently under active development.
Contribution guidelines will be added after public beta release.


---
