# Agentic Fraud Risk Detection Pipeline

An applied machine learning system for detecting fraudulent transactions using transaction-level risk modeling, adaptive routing logic, and fallback business-rule escalation.

---

## Overview

This project demonstrates a fraud risk detection workflow for transaction data, combining machine learning classification with agentic decision logic for automated approval, blocking, and manual review.

The system predicts fraud probability for each transaction, assigns interpretable risk levels, and routes borderline cases through a fallback review layer using additional business signals. Performance is evaluated using precision, recall, F1-score, and ROC-AUC.

---

## Key Features

- **Synthetic transaction risk dataset** generation  
- **Fraud classification model** using Random Forest  
- **Risk probability scoring** for each transaction  
- **Threshold-based routing** into auto-approve, manual review, and auto-block  
- **Fallback rule escalation** for suspicious medium-risk transactions  
- **Evaluation-driven design** using PRF and ROC-AUC metrics  
- **Feature importance analysis** for key risk signals  

---

## Problem Statement

Fraud prevention systems must balance:

- catching high-risk transactions  
- minimizing false positives  
- routing uncertain cases efficiently  
- scaling decisions across large transaction volumes  

This project addresses those challenges using an **agentic fraud decision pipeline**.

---

## Pipeline Architecture

```text
Transaction Data
   ↓
Feature Engineering
   ↓
Fraud Classification Model
   ↓
Fraud Probability Score
   ↓
Risk Band Assignment
   ↓
Routing Decision
   ├── Auto Approve
   ├── Manual Review
   └── Auto Block
   ↓
Fallback Rule Escalation
   ↓
Final Agentic Decision
   ↓
Evaluation (Precision, Recall, F1, ROC-AUC)

**Core Features Used**
• Transaction Amount
• Account Age
• Previous Transaction Count
• Device Trust Score
• Location Mismatch
• High-Risk Merchant Flag
• Multiple Failed Attempts
• Night Transaction Indicator

**Evaluation**

The system is evaluated using:

• Precision
• Recall
• F1-score
• ROC-AUC
**Example Insight**
• Baseline model predicts fraud labels directly
• Agentic routing expands coverage for uncertain medium-risk transactions
• Fallback business signals improve review prioritization

**Skills Demonstrated**
• Fraud Detection
• Risk Modeling
• Classification
• Precision / Recall Tradeoff Analysis
• Agentic Routing Logic
• Evaluation-driven ML Systems
• Feature Importance Analysis

Relevance to Industry

This project aligns with real-world problems in:

• Buyer Risk Prevention
• Trust & Safety Systems
• Fraud Detection
• Transaction Monitoring
• Automated Risk Decisioning

**Recruiter-Facing Summary**

Built an agentic fraud risk detection pipeline using transaction-level ML scoring, threshold-based routing, and fallback business-rule escalation to support automated approval, blocking, and manual review decisions.

**Future Improvements**
• Add anomaly detection models
• Incorporate temporal transaction sequences
• Add explainability for fraud decisions
• Extend to real-time streaming inference
• Build Streamlit dashboard for case monitoring
