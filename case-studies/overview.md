# Case Studies Overview  
Safety-Critical AI System Governance in Practice

---

## Purpose of the Case Studies

The case studies in this folder demonstrate how the **EvalOps, Operations, and Governance system** documented in this repository operates in real safety-critical scenarios.

Their purpose is not to showcase model behavior or individual failures, but to show how **risk is detected, evaluated, escalated, governed, and learned from** using predefined rules.

Each case study represents a full, end-to-end governance loop:
Evaluate → Incident → RCA → Decision → Monitoring → Improvement.

---

## Why Case Studies Exist Separately

The repository contains many formal artifacts:
- Evaluation Charters and Frameworks  
- Severity Models and Decision Logic  
- Monitoring and Incident Processes  

Case studies serve a different role.

They act as a **compression layer**, translating multiple internal artifacts into a single, coherent narrative that demonstrates judgment under real risk.

Without case studies, the system is theoretical.  
With case studies, the system is proven in operation.

---

## Structure of Each Case Study

Each case study follows the same governance-consistent structure:

1. Context and risk domain  
2. Initial observation and trigger  
3. EvalOps classification and severity assignment  
4. Incident creation and escalation  
5. Reproducibility assessment  
6. Root Cause Analysis  
7. Mitigation and validation  
8. Decision outcome (ship / conditional ship / no ship)  
9. Loop closure and learning  

This consistency ensures that cases are comparable and auditable.

---

## Case Study Index

### Case Study 1: Medical Safety (Non-Diagnostic Risk)

**Focus**
- Safety-critical medical information without diagnosis or treatment
- Risk arising from misleading reassurance and lossy simplification

**Governance Question**
- Can non-diagnostic framing still plausibly delay care or cause harm?

**What This Case Demonstrates**
- Severity assignment based on user impact, not tone  
- Escalation of subtle but high-risk behavior  
- Conditional ship decisions with bounded residual risk  

[medical-safety-case](https://drive.google.com/file/d/16mb45v7HVFQnm6Hszp3P4tWzwuE1iuVP/view?usp=drive_link)

---

### Case Study 2: Legal & Compliance Safety

**Focus**
- Legal and compliance-adjacent information
- Risk arising from over-authoritative framing and implicit guidance

**Governance Question**
- Can structure and tone influence legal or compliance decisions without explicit advice?

**What This Case Demonstrates**
- Actionability leakage without direct instructions  
- High-severity classification driven by decision influence  
- Governance of residual legal risk through framing controls and monitoring  

[legal-safety-case](https://drive.google.com/file/d/1CjX16uXgik5EIYkdDovwBTRVYq0KUSAN/view?usp=drive_link)

---

## What These Case Studies Do Not Show

To preserve safety, privacy, and clarity, the case studies do not include:
- Raw prompts or transcripts  
- Internal metrics or tooling  
- Model internals or training data  
- User-identifying information  

They are **public-safe narrative syntheses**, not raw logs.

---

## Relationship to the Rest of the Repository

The case studies do not introduce new rules or frameworks.

They strictly apply:
- EvalOps definitions and severity models  
- Operations processes and escalation rules  
- Governance decision logic and risk acceptance principles  

If a behavior is classified or a decision is made in a case study, the justification can be traced directly to documented artifacts elsewhere in the repository.

---

## Final Note

Together, these case studies demonstrate **AI System Governance in motion**.

They show how difficult, ambiguous, and high-impact situations are handled using discipline rather than intuition, and how safety decisions remain transparent, defensible, and accountable.

They are intended to be read alongside the Executive Summary and Governance documents to understand not just *what* decisions were made, but *how* and *why*.

---

## Status

Case Studies: Final  
Framework Alignment: Verified  
Public Safety Review: Passed  
