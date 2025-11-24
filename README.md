# SentriAI — AI-Powered Early Dropout Prediction System (Prototype)

SentriAI is a lightweight, low-code prototype that simulates an early-warning system for student dropout risk. It combines synthetic data, AI-generated predictions, a compact admin dashboard, and design assets so schools can quickly evaluate the value of proactive student retention workflows.

Table of Contents
- [Product Overview](#product-overview)
- [Problem Statement](#problem-statement)
- [Goals & Success Criteria](#goals--success-criteria)
  - [Primary Goals](#primary-goals)
  - [Success Indicators](#success-indicators)
- [Target Users](#target-users)
- [User Persona](#user-persona)
- [Core Features (MVP)](#core-features-mvp)
  - [A. Landing Page](#a-landing-page)
  - [B. Admin Dashboard](#b-admin-dashboard)
  - [C. Student List](#c-student-list)
  - [D. Student Profile](#d-student-profile)
  - [E. Risk Score Breakdown](#e-risk-score-breakdown)
  - [F. Alerts Center](#f-alerts-center)
  - [G. Intervention Suggestions](#g-intervention-suggestions)
- [Workflow / Solution Approach](#workflow--solution-approach)
  - [Simulation & Design Blueprint](#simulation--design-blueprint)
  - [Create Synthetic Dataset](#create-synthetic-dataset)
  - [Build AI Prediction Logic](#build-ai-prediction-logic)
  - [Prototype in Lovable (UI generator)](#prototype-in-lovable-ui-generator)
  - [Figma Polish (Optional)](#figma-polish-optional)
- [Week 1 Deliverables](#week-1-deliverables)
- [Non-Goals (MVP Scope)](#non-goals-mvp-scope)
- [Risks & Mitigations](#risks--mitigations)
- [Tech Stack](#tech-stack)
- [Quick Start (How to demo the prototype)](#quick-start-how-to-demo-the-prototype)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Product Overview
SentriAI simulates AI-driven dropout-risk detection for school administrators. The prototype provides:
- synthetic student records,
- AI-generated risk scores and concise explanations,
- an admin dashboard with alerts and recommended interventions,
- deliverables suitable for product demos, pitches, or stakeholder feedback.

## Problem Statement
Schools often miss early warning signs due to fragmented data and manual review processes. Common drivers of dropout include:
- poor engagement,
- low attendance,
- academic decline,
- behavioral instability.

SentriAI demonstrates a low-cost, fast-to-build early-warning prototype that flags at-risk students and suggests next steps for intervention.

## Goals & Success Criteria

### Primary Goals
- Detect students with Low / Moderate / High dropout risk.
- Provide administrators visibility into risk trends and topline alerts.
- Surface concise "reason for risk" explanations and possible interventions.
- Produce assets for demos and stakeholder conversations.

### Success Indicators
- Working interactive prototype with plausible simulated predictions.
- Admin dashboard showing risk distribution and student profiles.
- Clear landing page explaining value and workflow.
- Presentation-ready visuals (Figma screens or polished mockups).

## Target Users
- School administrators
- Guidance counselors
- Learning coordinators

Needs: visibility into at-risk students, simple explanations, and actionable next steps.

## User Persona
Name: Mrs. Amaka Okorie  
Role: Student Affairs / School Administrator (32–40)  
Goals: identify at-risk students early, monitor cohorts, trigger interventions  
Pain points: scattered data, reactive processes, time-consuming manual reviews

## Core Features (MVP)
SentriAI focuses on an admin-centered MVP to show value quickly.

### A. Landing Page
- Short product overview and value proposition
- How risk prediction works (simple diagram)
- Call-to-action: "View Dashboard" / "Open Demo"

### B. Admin Dashboard
- Total students count
- Risk distribution chart (Low / Moderate / High)
- Quick alerts and high-risk student list

### C. Student List
- Search & filter by risk, class, grade
- Risk category badges and key metrics (attendance %, GPA, warnings)

### D. Student Profile
- Personal and academic details
- Attendance and GPA trends
- Behavioral score timeline
- AI-generated risk level with a plain-language explanation

### E. Risk Score Breakdown
- Contribution factors and weightings
- Trend over time (risk history)

### F. Alerts Center
- Students crossing risk thresholds
- Sudden drops in performance or behavior spikes

### G. Intervention Suggestions
- Personalized, actionable recommendations
- Parent engagement steps, academic support strategies, and follow-up reminders

## Workflow / Solution Approach

### Simulation & Design Blueprint
- Produce mock screens with Lovable to validate layout, routing, and key interactions.
- Keep the flow simple: Landing → Dashboard → Student List → Student Profile → Alerts.

### Create Synthetic Dataset
- Example fields: attendance_pct, gpa, behavior_score, warning_count, parent_engaged, risk_level
- Tools: Mockaroo, ChatGPT, or simple CSV generators.
- Ensure plausible ranges and simple historic trends for demo realism.

### Build AI Prediction Logic
- Use Airtable AI, Glide AI, or other low-code tools to simulate prediction outputs:
  - Input: CSV of synthetic student records
  - Output: risk_score, risk_label, explanation_text
- Standardize prompt templates and ranges to keep results stable.

### Prototype in Lovable (UI generator)
- Use generated dataset and simulated AI outputs to populate Lovable screens.
- Implement basic filters, routing, and alert rules inside Lovable.

### Figma Polish (Optional)
- Import Lovable screens into Figma and refine spacing, color system, and typography for pitch-ready visuals.

## Week 1 Deliverables
- Interactive web app demo (Lovable or equivalent)
- Polished Figma mockups for pitch/demo
- Landing page and guided demo flow
- Predictive simulation with dashboard and student profile screens
- Shareable demo link and presentation assets

## Non-Goals (MVP Scope)
- Real production ML models trained on live student data
- Live SMS/email notifications
- Student/parent login or mobile apps
- Handling real PII or deploying in production without governance

## Risks & Mitigations
- AI predictions inconsistent → fix dataset ranges and template prompts.
- Scope creep → limit MVP to admin-only features.
- Visual clutter → keep UI minimal and finalize in Figma.
- Data realism issues → enrich synthetic data with simple historic trends and edge-cases.

## Tech Stack
- Lovable — Web app generation & prototype routing
- Glide AI / Airtable AI — Prediction simulation engine
- Figma — Visual polish & pitch assets
- ChatGPT / Mockaroo — Synthetic data generation

## Quick Start (How to demo the prototype)
1. Prepare a synthetic dataset (CSV) with the fields described above.
2. Feed it into your chosen prediction engine (Airtable AI / Glide AI) with a stable prompt that returns:
   - risk_score (numeric), risk_label (Low/Moderate/High), explanation_text.
3. Import the dataset and prediction outputs into Lovable to create the landing page, dashboard, and profiles.
4. Optionally import Lovable screens into Figma and polish visuals for a pitch.

If you prefer, provide the CSV and I can draft prompt templates and a sample Lovable project structure.

## Contributing
Contributions and feedback are welcome. Suggested workflow:
1. Fork the repo
2. Create a branch: git checkout -b feat/your-feature
3. Add or update mock data, screens, or docs
4. Open a PR with a clear description and screenshots

Include tests or sample data where helpful.

## License
This project is available under the MIT License — see [LICENSE](./LICENSE).

## Contact
Maintainer: Vivian-hub-byte — https://github.com/Vivian-hub-byte  
For questions, feature requests, or running the demo, open an issue or message via GitHub.

---

Notes
- This README is tailored to a prototype built with low-code tools (Lovable, Glide/Airtable AI). If you want a README tied to a full-code implementation (Python/Flask/FastAPI + trained model), I can adapt this document and add setup/run instructions for that stack.
