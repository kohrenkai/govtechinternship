# University Marketplace Chatbot – Realistic Testing Approach

## Overview
This document outlines a realistic testing approach for the University Marketplace Chatbot, using structured test cases to ensure **accuracy, professionalism, safety, and reliability**. The approach applies to all test cases, including basic navigation, transaction support, safety guidelines, escalation triggers, and edge cases.

---

## Test Case Structure
Each test case includes:
- **id**: Unique identifier
- **category**: Test category (navigation, transaction, safety, escalation, edge)
- **input**: User query
- **expected_elements**: Key items that must appear in the response
- **success_criteria**: Defines when the test passes
- **edge_case**: True if the query is unusual or ambiguous

---

## Step 1: Prepare Test Environment
1. Use a test account on the chatbot platform.
2. Ensure the chatbot is running the latest version.
3. Prepare test tools for sending queries and capturing responses.

---

## Step 2: Execute Test Cases
1. Send the **input** from the test case to the chatbot.
2. Capture the chatbot’s response.

---

## Step 3: Verify Response
1. Check for **all expected elements** in the response.
   - Example for `nav_001`:
     - Posting steps ✅
     - Pricing guidance ✅
     - Photo requirements ✅
2. Ensure the response meets the **success criteria**:
   - Clear, step-by-step instructions
   - Polite and professional tone
3. For edge cases (`edge_case: true`):
   - Verify the bot asks clarifying questions or politely declines irrelevant queries.
4. For escalation triggers (`[ESCALATION_REQUIRED]`):
   - Ensure the bot logs the issue or notifies moderators appropriately.

---

## Step 4: Test Variations
- Rephrase queries to confirm **robustness**:
  - e.g., `"I want to sell my textbook"` → should yield same expected elements as `nav_001`.
- Include minor spelling or phrasing changes to test **natural language understanding**.
