# EvalOps Overview  
**Evaluation Operations for Google Gemini**

---

## Purpose of the EvalOps Layer

The EvalOps layer defines how **model behaviour is evaluated** in this project.

Its purpose is to establish **clear, consistent, and auditable rules** for identifying failures, assessing severity, and interpreting risk **before any operational decisions are made**.

EvalOps ensures that judgments about model behaviour are:
- Not subjective
- Not reactive
- Not influenced by downstream outcomes

In this project, EvalOps serves as the **foundation for monitoring, incident handling, and decision-making activities**.

---

## What EvalOps Means in This Project

EvalOps is treated as a discipline focused on **behavioural correctness and user risk**, not model capability or intelligence.

The EvalOps layer answers the following questions:

- What model behaviours matter from a **safety, trust, and reliability** perspective
- What constitutes a **failure** versus acceptable behaviour
- How **severity** is determined based on potential user impact
- When an observation becomes an **incident**
- What **evidence** is required to support a judgment or decision

EvalOps does **not** attempt to:
- Optimize the model
- Explain internal mechanisms

Its role is to define **how behaviour is judged** in a consistent and defensible way.

---

## Relationship to the Project Charter

The EvalOps layer operates under constraints defined in the **Project-Level Charter**.

It inherits the following principles:

- Frozen definitions
- Evidence-based reasoning
- Separation between evaluation and decision authority

Once execution begins, EvalOps **does not**:
- Change scope
- Redefine risk domains
- Adjust severity thresholds

All EvalOps documents align directly with broader project objectives of **safety, reliability, and trust**.

---

## Scope of EvalOps

EvalOps covers evaluation of model outputs across the following areas:

- Safety-critical behaviour in high-risk domains, including:
  - Medical scenarios
  - Legal scenarios
  - Financial scenarios
  - Self-harm–related scenarios
  - Dangerous or hazardous action scenarios

- Hallucination and factual reliability, with a focus on:
  - Confident but incorrect claims
  - Unverifiable assertions

- Source and citation integrity, particularly where:
  - Sources are missing
  - Sources are fabricated
  - Citations may mislead users

EvalOps evaluates responses to **realistic user prompts**.  
It does **not** focus on adversarial stress testing or exploit discovery.

---

## What EvalOps Does Not Cover

EvalOps explicitly excludes:

- Model training or fine-tuning decisions
- Benchmarking or leaderboard comparisons
- Infrastructure or system performance metrics
- Fairness, bias, or demographic impact analysis
- Detection of user intent or misuse motivation

These exclusions are intentional and ensure EvalOps remains focused on **observable behaviour and operational relevance**.

---

## How EvalOps Is Structured

EvalOps documentation reflects the **lifecycle of evaluation judgment**, moving from intent to interpretation.

Documents should be read in sequence:

1. **Evaluation Charter**  
   Defines why and what is evaluated  
   [evaluation-charter](https://drive.google.com/file/d/1URrrol196Av2VfwJI6hqMj5TSWpIzUje/view?usp=drive_link)

2. **Evaluation Framework**  
   Establishes fixed categories and boundaries  
   [eval-framework](https://drive.google.com/file/d/1FgZwgLClmEor4C87MzCTBMum2TeEsQeJ/view?usp=drive_link)

3. **Category Plan**  
   Maps evaluation areas to risk focus  
   [category-plan](https://drive.google.com/file/d/1_RTfUgdTzExoIg4-BCXcqjUxeVitaMg5/view?usp=drive_link)

4. **Minimum Expected Outputs**  
   Defines what constitutes a complete evaluation  
   [minimum-expected-outputs](https://drive.google.com/file/d/1Z1wVMF9vMUNvDykMROwIsqDaSAoS5MyJ/view?usp=drive_link)

5. **Severity & Scoring Interpretation**  
   Explains how impact is assessed  
   [scoring-interpretation](https://drive.google.com/file/d/18-ysBjklov_3u8NVDcT96wIf55f2RFkI/view?usp=drive_link)

6. **Failure Pattern Mapping**  
   Abstracts recurring risk behaviours  
   [failure-pattern-mapping](https://drive.google.com/file/d/1lQE7eqms2XRCV19qwf9QLGfKyQtVqzgv/view?usp=drive_link)

Each document builds on the previous one.

---

## Severity and Judgment Philosophy

Severity reflects **potential user impact**, not:
- Model intent
- Frequency of occurrence

Key principles:

- A single high-impact behaviour can outweigh many low-risk observations
- Reproducibility increases confidence but does not automatically change severity
- EvalOps prevents:
  - Overreaction to minor issues
  - Underreaction to subtle but dangerous patterns

---

## Outputs of the EvalOps Layer

EvalOps produces structured outputs that feed directly into Operations:

- Clearly defined evaluation criteria
- Consistent severity classifications
- Documented failure patterns
- Evaluation summaries suitable for leadership review

These outputs are **inputs**, not final decisions.  
They support monitoring, incident handling, and **ship / no-ship recommendations**.

---

## How to Use This Section

Readers new to the project should start with this document, then proceed to the **Evaluation Charter**.

Each document can be read independently, but full intent is best understood when read as a **complete system**.

This section is written to be **public, professional, and educational**.  
Sensitive prompts, raw transcripts, and internal decision logs are intentionally excluded.

---

## Status

- **EvalOps Status:** Defined and executed  
- **Definitions and severity rules:** Frozen  
- **Role in project:** Judgment foundation for operations and governance  

---
