# PROCESS LOG

This log documents my step-by-step thought process while completing the University Marketplace Chatbot assessment.  
It captures how I approached each part, the decisions made, and key reflections.

---

## Setup
- Read the assessment instructions carefully and noted all required deliverables.  
- Created a GitHub repository and set up the folder structure based on the specification.  
- Sketched a rough workflow in my notes to stay organized.
- Refreshed my knowledge on chatbots by reviewing old mateirals of workshops i attended earlier in the year

---

## Part 1 – Prompt Engineering
- Reviewed requirements: role definition, task specifications, conditional logic, safety guardrails, and university context.  
- Applied modern prompt engineering best practices: clarity, role assignment, step-by-step logic, and structured formatting.  
- Wrote `prompt.md` using Markdown.  
- Designed scenarios to support buyers, sellers, new users, and cases involving safety concerns.  
- Added escalation pathways to human moderators for policy violations.  
- Documented design choices and trade-offs in `prompt-analysis.md`.  

---

## Part 2 – Golden Test Design
- Identified required categories: **Basic Navigation, Transactions, Safety, Escalation, Edge Cases**.  
- Created a set of structured golden test cases in `test-cases.json` to validate chatbot responses.  
- Ensured each test had input, expected elements, success criteria, and an edge flag.  
- Included a nonsense input case to test chatbot resilience to unclear queries.  
- Wrote `testing-framework.md` to outline a realistic testing approach
- Key decision: organize test cases by category to ensure balanced coverage. (4 cases of each category)

---

## Part 3 – Automation & Update Process
- Reviewed requirements: version control, automated testing, deployment workflow, rollback, and policy approval.  
- Drafted `update-process.md` to explain the update pipeline.  
- Designed a workflow diagram showing developer PRs, automated tests, moderator approval, deployment, and rollback.    
- Wrote `automation-concept.py` as pseudo-code, outlining how tests, deployment, and rollback could be automated.  
- Key decision: keep automation conceptual but realistic

---

## Part 4 – Marketplace Domain Knowledge
- Reflected on real-world challenges in student marketplaces, including safety, trust, and seasonal usage spikes.  
- Documented insights in `marketplace-insights.md` across four areas: user pain points, safety/trust, seasonal patterns, and university system integration.  

---

## Wrap-Up
- Wrote `README.md` to summarize the entire approach, including assumptions, reflections, and next steps.  
- Verified all deliverables were present and properly structured:
  - `prompt.md`, `prompt-analysis.md`, `test-cases.json`, `testing-framework.md`,  
  - `update-process.md`, `automation-concept.py`, `marketplace-insights.md`, `PROCESS_LOG.md`.  
- Ensured formatting and documentation were consistent and professional.

---