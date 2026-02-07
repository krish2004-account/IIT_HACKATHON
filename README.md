# Conversational Causal Analysis with Multi-Turn Context

## 📌 Problem Overview
Large-scale conversational systems generate multi-turn dialogues between agents and customers.
While some conversations are labeled with outcome events such as **Escalation, Refund, or Fraud**, the **causal conversational factors** leading to these outcomes are not explicitly recorded.

This project addresses this gap by:
- Identifying dialogue-level causal factors
- Extracting concrete, traceable evidence from conversations
- Supporting multi-turn, context-aware analytical queries

---

## 🎯 Objectives
- Move from simple outcome detection to **causal explanation**
- Provide **interpretable, evidence-based outputs**
- Enable **interactive exploration** through follow-up queries
- Maintain deterministic and faithful reasoning

---

## 🧠 Task Overview

### ✅ Task 1: Query-Driven Causal Explanation
Given a natural-language analytical query such as:

> **“Why do escalations occur?”**

the system:
- Identifies conversations labeled with escalation outcomes
- Detects causal dialogue patterns (e.g., repeated complaints, frustration)
- Extracts supporting dialogue text as evidence
- Produces a structured causal explanation

#### Output
- Outcome event (e.g., Escalation)
- Identified causal factors
- Supporting evidence (dialogue text)
- Transcript IDs

---

### ✅ Task 2: Multi-Turn Context-Aware Query Handling
Task 2 extends Task 1 by enabling **follow-up analytical queries** that depend on prior system responses.

The system:
- Maintains explicit and deterministic conversational context
- Reuses previously identified causes and evidence
- Ensures consistent causal reasoning across multiple turns

#### Example Follow-up Queries
- “What is the main reason?”
- “Which customer behavior contributed most?”
- “Give other similar examples”

---

## 📊 Dataset Description
The dataset consists of multi-turn conversational transcripts between customers and agents.
Each transcript includes:
- Transcript ID
- Speaker roles (Customer / Agent)
- Ordered dialogue turns
- Outcome labels (e.g., Escalation, Refund)

No turn-level ground-truth annotations are provided, motivating **evidence-based evaluation** rather than token-level accuracy.

---

## ⚙️ System Design
- Rule-based causal analysis (no black-box machine learning models)
- Deterministic and interpretable logic
- Explicit context storage for multi-turn interaction
- Evidence traceability to concrete dialogue text

---

## 📈 Evaluation Metrics

### ID Recall (Evidence Accuracy)
Measures whether the system retrieves all transcript IDs associated with a queried outcome event.
### Evidence Support Rate
Measures whether at least one supporting dialogue segment is identified for each outcome-labeled conversation.

---

## 📁 Project Structure
---

## 🔧 Environment Setup

This project is designed to run in **Google Colab or a local Python environment**.

### Requirements
- Python 3.x
- Required libraries:
  - json
  - collections
  - numpy
  - matplotlib
  - scikit-learn

No additional installation is required when using Google Colab.

---

## ▶️ How to Run

### Option 1: Local Execution
```bash
python main.py
