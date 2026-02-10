# Governance

This folder defines the **decision authority layer** of the AI System Governance model implemented in this repository.

While EvalOps defines how behavior is evaluated and Operations defines how issues are monitored and handled, **Governance defines how decisions are made, justified, recorded, and audited**.

The documents in this folder establish:
- Severity authority
- Release gating logic
- Risk acceptance discipline
- Audit readiness requirements

Together, they ensure that AI safety decisions are **explicit, defensible, and accountable**, rather than implicit or ad hoc.

---

## Purpose of the Governance Layer

The governance layer exists to answer four critical questions:

1. How severe is a given failure, and why?
2. What decisions does that severity require?
3. What risk, if any, is being explicitly accepted?
4. Can these decisions withstand internal or external scrutiny?

Governance does not aim to eliminate all risk.  
It ensures that **risk is consciously evaluated, documented, and owned**.

---

## Files in This Folder

### [severity-model](https://drive.google.com/file/d/1c6LRXbWyzkJHj3MUN4pptr1AK7y1PwgZ/view?usp=drive_link)

Defines how failures are classified by severity based on **plausible user impact**, not tone, intent, or disclaimers.

The severity model:
- Establishes non-negotiable thresholds
- Prevents downscoping for convenience
- Preserves historical severity decisions
- Acts as the backbone for all release and escalation logic

All other governance decisions depend on this model.

---

### [ship-no-ship-logic](https://drive.google.com/file/d/1WAkMwQM5WOHFQA757Dsd_UethSBUAIKK/view?usp=drive_link)

Defines how severity and evidence translate into **release decisions**.

This document specifies:
- Automatic no-ship conditions
- Conditions for conditional ship
- Required evidence before release eligibility
- The relationship between mitigation, residual risk, and monitoring

Ship / no-ship decisions are governed by rules, not preference.

---

### [risk-acceptance-philosophy](https://drive.google.com/file/d/1usdrkEf8OYs0wEMTdGpBKAULC0_wPedE/view?usp=drive_link)

Defines when and how **residual risk may be accepted**, and when it must not be.

This document makes explicit that:
- Risk acceptance is not risk elimination
- Certain classes of risk are never acceptable
- Accepted risk must be documented, time-bound, and owned
- Risk acceptance cannot override severity or safety blocks

This prevents silent or accidental normalisation of risk.

---

### [audit-readiness](https://drive.google.com/file/d/14c39RHOMkp9EYAF_awso7SSKLX9uBk5S/view?usp=drive_link)

Defines the requirements for **traceability, evidence, and decision integrity**.

Audit readiness ensures that:
- Every decision can be reconstructed
- Severity assignments are justified
- Disagreements and challenges are recorded
- No retroactive edits obscure historical outcomes

Audit readiness is treated as a **system property**, not a reporting exercise.

---

## Relationship to Other Repository Layers

The governance layer depends on, but is distinct from:

- **EvalOps**  
  Provides the definitions, categories, and severity inputs used by governance.

- **Operations**  
  Provides incidents, RCA findings, and monitoring signals that inform governance decisions.

Governance does not redefine evaluation outcomes or operational facts.  
It **interprets them into decisions and accountability**.

---

## Governance Principles

The governance layer in this repository is built on the following principles:

- Severity reflects potential harm, not confidence or intent
- Decisions are based on worst-case impact, not averages
- Risk acceptance must be explicit and reviewable
- Learning must be preserved, not overwritten
- Convenience must not weaken safety thresholds

When trade-offs exist, they are documented rather than hidden.

---

## Intended Audience

This folder is written for:
- Product and platform leaders responsible for release decisions
- AI safety and trust reviewers
- Risk, compliance, and audit stakeholders
- Evaluators assessing governance maturity

It is not written for end users or model developers.

---

## Status

Governance Framework: Defined and Frozen  
Severity Model: Active  
Ship / No-Ship Logic: Enforced  
Risk Acceptance Rules: Active  
Audit Readiness: Required  

This governance layer represents the **decision spine** of the AI System Governance model demonstrated in this repository.
