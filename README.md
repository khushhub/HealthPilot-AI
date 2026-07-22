#  Healthcare Appointment & Triage Assistant

> *"Because nobody should have to guess how urgent their symptoms are."*

An **NHS-inspired**, AI-powered healthcare platform that helps patients describe symptoms, receive an intelligent triage suggestion, and book the right appointment — all while giving admins a real-time pulse on clinic operations.

Built end-to-end as a portfolio project spanning **Data Analytics, Data Science, Machine Learning, Generative AI, and Full-Stack Engineering.**

---

##  Why this project exists

Healthcare shouldn't feel like a maze. Patients often don't know whether their symptoms need a routine check-up or urgent care — and clinics lose time and money to no-shows they can't predict.

This project simulates a smarter, calmer version of that experience: describe how you feel, get a sensible triage suggestion, book a slot, and chat with an AI assistant grounded in trusted public guidance — no guesswork, no dead ends.

>  **Educational project only.** Built with public and synthetic data. Not affiliated with the NHS. Not a substitute for real medical advice. **In an emergency, always call 999 (UK) or your local emergency number.**

---

##  What it actually does

| Feature | What it means for the user |
|---|---|
|  **Symptom entry** | Describe symptoms in plain language |
|  **AI triage suggestion** | Get sorted into Self-care, Routine GP, Urgent, or Emergency |
|  **Appointment booking** | Find and book the right slot instantly |
|  **AI health chatbot** | Ask general health questions, answered with cited sources (RAG) |
|  **Admin dashboard** | Live view of appointments, no-show risk, and daily trends |
|  **Emergency escalation** | Red-flag symptoms trigger an immediate safety message |

---

##  How it's built

```
Patient
   ↓
Frontend (React + Next.js)
   ↓
Backend (FastAPI)
   ├── PostgreSQL Database
   ├── Machine Learning Models
   └── AI Chatbot (RAG)
```

A clean, layered system where every piece has one job — and does it well.

---

##  Tech stack at a glance

| Layer | Tools |
|---|---|
| **Frontend** | React, Next.js, TypeScript, Tailwind CSS |
| **Backend** | FastAPI, JWT Auth, Pydantic |
| **Database** | PostgreSQL |
| **Machine Learning** | scikit-learn, XGBoost |
| **Generative AI** | OpenAI / Anthropic API, LangChain, FAISS |
| **DevOps** | Docker, GitHub Actions, Render |
| **Testing** | pytest, Jest |

---

##  The datasets behind it

No real patient data — ever. Just public and synthetic sources:

- **Medical Appointment No-Shows** (Kaggle) — ~110k real-world booking records
- **Synthea** (MITRE) — fully synthetic patient generator
- **NHS England Open Data** — GP appointment statistics
- **NICE Clinical Knowledge Summaries** — grounding text for the AI chatbot

---

##  Built responsibly

-  Only public/synthetic data, always
-  No secrets or credentials ever committed
-  Prompt-injection safeguards on the chatbot
-  Visible medical disclaimer in every screen
-  UK GDPR-style data handling, even for demo data

---

##  Project structure

```
nhs-triage-assistant/
├── .github/
│   └── workflows/
│       └── ci.yml
├── backend/
│   ├── app/              (routes, models, schemas, services)
│   ├── tests/
│   └── requirements.txt
├── frontend/
│   ├── app/               (Next.js pages/components)
│   ├── tests/
│   └── package.json
├── ml/
│   ├── notebooks/         (EDA, feature engineering, modelling)
│   ├── models/            (saved model artifacts - or Git LFS)
│   └── src/               (training & evaluation scripts)
├── genai/
│   ├── rag_pipeline/      (chunking, embedding, retrieval)
│   └── prompts/           (system prompts, guardrail templates)
├── data/
│   ├── raw/                (gitignored - download scripts only)
│   └── processed/          (small samples only, if any)
├── docs/
│   ├── architecture.png
│   ├── DATA_SOURCES.md
│   └── data_dictionary.md
├── docker-compose.yml
├── .gitignore
├── LICENSE
└── README.md
```

---

##  Author

**Khushi**


<p align="center">
  <em>Made with curiosity, careful data handling, and a healthy respect for what AI shouldn't be trusted to decide alone.</em>
</p>
