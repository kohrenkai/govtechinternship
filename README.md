# University Marketplace Chatbot

This repository contains my submission for the GovTech **University Marketplace Chatbot – Intern Take-Home Assessment**.  

The project demonstrates my approach to **prompt engineering**, **testing methodology**, **automation design**, and **domain understanding** of student marketplaces.

---

## Introduction and Approach Overview

I approached this assessment in four main stages:  

1. **Prompt Engineering**  
   - Designed a structured system prompt (`prompt.md`) using Markdown formatting.  
   - Defined roles, tasks, safety guardrails, and conditional logic using the TCREI framework.  
   - Considered multiple user scenarios (buyers, sellers, new users, and safety issues).  

2. **Golden Test Design**  
   - Created `test-cases.json` with 20 structured cases covering navigation, transactions, safety, escalation, and edge scenarios.  
   - Documented the testing approach in `testing-framework.md`.  

3. **Automation & Update Process**  
   - Developed a version-controlled workflow (`update-process.md`) supported by a diagram (`resources/update-workflow.png`).  
   - Implemented pseudo-code (`automation-concept.py`) for automated testing, deployment, and rollback.  

4. **Marketplace Domain Knowledge**  
   - Analyzed student marketplace challenges in `marketplace-insights.md`.  
   - Linked pain points to chatbot requirements, including navigation, safety, seasonal patterns, and integration with university systems.  

---

## How to Review Each Component

- **Prompt design**: `prompt.md`, `prompt-analysis.md`  
- **Testing framework**: `test-cases.json`, `testing-framework.md`  
- **Update workflow**: `update-process.md`, `automation-concept.py`, `resources/update-workflow.png`  
- **Marketplace insights**: `marketplace-insights.md`  
- **Process documentation**: `PROCESS_LOG.md`  

---

## Assumptions Made

- Users are verified via **valid university emails** (`@e.ntu.edu.sg`) to restrict access to the campus community.  
- Users primarily buy, sell, or trade items within the NTU campus community.  
- Users are generally familiar with campus locations (North Spine, South Spine, canteens, meet-up zones).  
- Users will follow basic safety and behavioral guidelines.  
- Transactions are **peer-to-peer**, with no third-party payment or shipping support.  

---

## Time Breakdown

- **Prompt Engineering**: ~45 minutes  
- **Golden Test Design**: ~25 minutes  
- **Automation & Update Process**: ~20 minutes  
- **Marketplace Insights**: ~15 minutes  
- **Documentation & Cleanup**: ~15 minutes  

**Total**: ~2 hours  

---

## Next Steps (If This Were a Real Project)

- Expand golden test cases to cover **multi-turn conversations**.
- More test cases with similar phrasning as existing cases to refine chatbot.
- Integrate automated testing with **GitHub Actions CI/CD**.  
- Prototype a live chatbot interface using the designed prompt.  
- Add a continuous feedback loop to log failed queries for prompt refinement.  
- Collaborate with policy teams to ensure chatbot moderation aligns with university rules.  

---

## Personal Reflection

The most challenging component was **prompt engineering**. As a beginner, I revisited what I learned in an earlier LLM Workshop and applied it to cover multiple user roles, enforce safety, and anticipate edge cases. Applying best practices—role definition, structured outputs, and guardrails—was a valuable learning experience.  

---

## Alternative Approaches Considered

1. **Full rule-based responses instead of few-shot prompting**  
   - Rejected because rule-based systems are rigid, harder to maintain, and less adaptable to varied queries.  

2. **Fully automated escalation**  
   - Rejected because it could misinterpret context and make unsafe decisions; human oversight is required.  

3. **Free-form text responses instead of structured outputs**  
   - Rejected because free-form text is harder to parse, inconsistent, and less testable against golden test cases.  

---

## Personal Experience with University Marketplaces

I have personally used student marketplaces to buy a used router and sell an old fridge. Challenges I encountered included:  

- Negotiating fair prices  
- Last-minute cancellations  
- Ensuring safe and reliable meet-ups  

These experiences informed my focus on **safety guardrails**, **clear navigation**, and **seasonal adaptability** in the chatbot design.
