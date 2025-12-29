# HackZenith Project
![Snapshot](SnapShots/Snapshot1.png)
## Problem Statement
Colleges struggle with high inquiry volumes during peak times such as admissions or registration, leading to long wait times, missed calls, and overburdened staff. Limited hours of human receptionists result in delayed responses for students, parents, and visitors, while manual processes cause scheduling errors and miscommunications. Resource constraints in smaller institutions exacerbate these issues, reducing student satisfaction and engagement. Coordinating appointments and counseling sessions manually leads to conflicts, no-shows, and double-bookings, wasting time and resources.
## Solution
AI receptionists uses NLP for multilingual call handling, instant calendar syncing for bookings, and escalations for complex needs, saving 30% staff time. They provide analytics for insights, crisis alerts, and personalized responses, scaling effortlessly for enrollment surges while integrating with campus CRMs.
- **Staff Efficiency:**\
Frees personnel from routine calls, saving up to 30% time for complex tasks like counseling.
- **Scalability:**\
 Manages inquiry spikes during admissions without added costs, plus analytics for service improvements.
- **Enhanced Engagement:**\
 Offers crisis alerts, event coordination, and accessibility features, boosting student satisfaction and retention.
## How It Solves The Problem
- 24/7 availability: instant triage and answers anytime, eliminating queue bottlenecks.
- Reduced manual enquiries: automates routine tasks (current scholarship details, providing placement stats), cutting repetitive workload.
- Faster resolution & routing: structured actions (send_email, fetch_college_api, search_scholarship) speed fulfillment and escalate when needed.
- Trustworthy responses: uses college data; confidence score and provenance reduce hallucination risk.
## Features
- **Instant college Q&A:** Fast, accurate answers to admissions, departments, placements, and general college queries.
- **Lightweight context management:** Remembers the last action taken  by the user (e.g., fetched placements, searched scholarships) to maintain continuity across follow-up questions.                
- **Scholarship discovery & guidance:** Provides details of available scholarships, SVMCM information, and application schedules.
- **Agent-driven mailing system:** Automatically drafts and sends emails for reporting issues, enquiries, or personal requests to the correct department.
- **Official college data retrieval:** Fetches structured college information (addmissions, placement records, department details) via maintained APIs / curated datasets.
- **Resilient AI architecture:** 3-retry strategy with automatic model switching and timeouts to ensure responses even during model failures.
- **Efficient & cost-aware API usage:** Optimized prompting, selective model calls, and lightweight orchestration to minimize latency and API usage.
- **Confidence-aware decision making:** Each action includes a confidence score to validate intent and handle uncertain queries safely.

## Used Technologies
- Google-generative AI (Python SDK)
- Gemini Models (Gemini-2.5-Flash & Gemini-2.5-Flash-Lite)
- SMTP Server (smtp.gmail.com port:587)
- FastAPI (Backend)
- React (Frontend)
