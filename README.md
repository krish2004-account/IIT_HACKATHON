# Conversational Transcript Analysis and Memory-Based QA System

## Project Description
This project analyzes customer–agent conversational transcripts to identify **customer escalation causes** and to build a **memory-based conversational question answering (QA) system**.  
The solution is designed using **rule-based logic** to ensure transparency, simplicity, and ease of understanding for academic evaluation.

---

## Dataset
- **File:** `Conversational_Transcript.json`
- **Format:** JSON
- **Content:** Customer and agent conversation transcripts

Each transcript contains a unique ID and a sequence of dialogue turns between a customer and an agent.

---

## Project Structure
├── source_code.ipynb
├── Conversational_Transcript.json
└── README.md


---

## Task 1: Escalation Detection and Explanation
The system analyzes conversations to determine why an escalation occurred.  
Common escalation reasons include:
- Explicit escalation requests
- Repeated unresolved issues
- Customer frustration
- Delayed resolution

For each transcript, the system provides:
- Identified escalation causes  
- Supporting textual evidence  
- A confidence score  

Visual analysis is also included to show cause frequency and confidence distribution.

---

## Task 2: Memory-Based Conversational QA System
A simple conversational QA system is implemented to demonstrate **context retention** across multiple queries.

### Key Features
- Retrieves relevant transcripts for initial questions
- Stores retrieved information in memory
- Uses memory for follow-up questions to reduce redundant retrieval

This approach improves efficiency and simulates real conversational behavior.

---

## Model Information
This project does **not** use machine learning or deep learning models.

Instead, it uses:
- Rule-based decision logic
- Keyword and pattern matching
- Lightweight retrieval techniques

This ensures full interpretability and fast execution.

---

## Tools and Technologies
- **Language:** Python  
- **Libraries Used:**
  - `json`
  - `collections`
  - `matplotlib`

---

## How to Run:-
1. Ensure `Conversational_Transcript.json` is in the project directory
2. Open the notebook:
   ```bash
   jupyter notebook source_code.ipynb
3.Run all cells in sequence

## Results:-

1.Clear identification of escalation causes

2.Transparent confidence-based explanations

3.Efficient memory reuse in conversational QA

4.Graphical validation of system behavior

## Team Members:-

1.Krish Mukherjee

2.Somalin Samal

3.T Subha Shree

4.Sanskruti Singha
