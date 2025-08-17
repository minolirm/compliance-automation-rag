# 🛡️ Case Study: Compliance Automation with RAG + ML + LLMs
A Retrieval-Augmented Generation (RAG) pipeline for automated compliance evaluation of regulations and organizational policies.

## 📌 Background & Problem
Organizations in regulated sectors (finance, healthcare, education, etc.) must constantly ensure that their internal policies align with external regulations.  

- Traditional compliance reviews are **manual, time-consuming, and error-prone**.  
- Policies and regulations change frequently, making static rule-based or fine-tuned ML models **costly to maintain**.  

**Business Challenge:** Automate compliance evaluation so auditors and policy teams can quickly identify gaps, reduce manual effort, and improve audit readiness.  

---

## 🎯 Objectives
- Automate the process of comparing **organizational policies vs. regulations**.  
- Classify regulatory clauses as:  
  &emsp; ✅ Fully Addressed  
  &emsp; ⚠️ Partially Addressed  
  &emsp; ❌ Not Addressed  
- Generate **structured, interpretable reports** for compliance officers.  
- Ensure the solution is **scalable, transparent, and adaptable** across domains.  

---

## 🏗️ Solution Approach
Designed and implemented a **hybrid Retrieval-Augmented Generation (RAG) pipeline** that ingests regulations and policies, retrieves relevant matches, and uses a **two-stage evaluation**:  

1. **ML Classifier** – Handles high-confidence cases efficiently.  
2. **LLM (via OpenAI API)** – Provides reasoning and classification for ambiguous cases.  
3. **LangChain Orchestration** – Connects the vector database, classifier, and OpenAI API to manage the entire workflow.  
4. **Human-in-the-Loop** – Ensures audit reliability when confidence is low.  


### 🔹 Architecture Diagram
📄 [View Architecture Diagram](solution_architecture.png)
