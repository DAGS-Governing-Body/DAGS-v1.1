# Changelog

All notable changes to the **Deployment AI Governance Standard (DAGS)** are recorded in this document.

This changelog documents version-to-version changes in the normative requirements, terminology, and structural architecture of the standard.

Where detailed narrative explanation is required, supplementary material may be provided in the **RELEASES** directory.

---

## v1.1 — 2026-03-11

**Status:** Published  
**Normative Status:** Additive Minor Release  
**Supersedes:** v1.0

---

## Summary

Version 1.1 extends the Deployment AI Governance Standard to address **agentic deployment environments** in which AI-enabled systems initiate and propagate consequential actions across multiple systems, services, and operational boundaries.

The **five-domain architecture** of the standard remains unchanged.

All controls introduced in **v1.0 (D1.1–D5.13)** remain in force without modification.

Version 1.1 introduces **14 new controls within Domain D3**, increasing the total number of normative controls from **57 to 71**.

---

## Normative Additions

### Domain D3 — Security and Controls

Version 1.1 introduces additional controls governing **authorization continuity**, **delegation integrity**, and **reconstruction of agentic execution paths**.

These controls extend deployment-layer governance to environments in which a single authorization event may initiate a sequence of consequential system actions across multiple systems.

---

### Authority Continuity Controls

**D3.19 – D3.22**

These controls govern preservation and enforcement of authorization constraints across **execution paths** spanning multiple systems.

Key governance requirements include:

- preservation of the original authorization scope  
- prohibition of implicit privilege expansion  
- revalidation of authority during execution path propagation  
- independent enforcement of authorization constraints across system boundaries  

---

### Identity and Delegation Controls

**D3.23 – D3.26**

These controls govern identity propagation and delegation integrity across execution paths.

Key governance requirements include:

- privilege scoping across delegated actions  
- credential propagation constraints  
- identity provenance verification  
- prevention of authority scope expansion during delegation  

---

### Execution Path Evidence Controls

**D3.27 – D3.32**

These controls establish evidence standards for reconstruction of **agentic execution paths**.

Required governance artifacts include:

- persistent execution path identifiers  
- authority lineage records  
- materiality threshold snapshots  
- irreversibility markers  
- chain terminal records  

Execution path governance applies only to system operations capable of producing **consequential state change**.

Internal model reasoning, intermediate planning steps, and computational processes without operational effect remain outside the scope of these controls.

---

## Normative Terminology Additions

Version 1.1 introduces five defined terms governing execution path governance:

- **Execution Path**  
- **Execution Path Initiation Event**  
- **Legibility Boundary**  
- **Planning Authority**  
- **Materiality Threshold**

These terms clarify governance obligations when authorized actions propagate across multiple systems or agents.

---

## Structural Clarifications

The following governance doctrines introduced in **v1.0** remain in force and unchanged in **v1.1**.

---

### Materially Affecting Behavior

The defined term **Materially Affecting Behavior** governs:

- change authorization thresholds  
- vendor update triggers  
- governance logging requirements  
- reconstruction obligations  
- ethical oversight escalation  

Materiality determinations must be **documented**, **attributable**, and **periodically reassessed**.

---

### Strategy vs Deployment Boundary

DAGS governs the **deployment layer of AI systems**, not organizational AI strategy.

However, enterprise strategy and ethical commitments define the **accountability perimeter** within which deployment governance operates.

---

### Operationalization of Ethical Constraints

Ethical commitments must be translated into **enforceable operational controls**, including:

- transparency of system purpose and limitations  
- explainability appropriate to system risk  
- fairness and non-discrimination safeguards  
- performance monitoring  
- human oversight capability  

Aspirational ethical statements without enforceable controls are insufficient.

---

### Governance Competence Requirement

Individuals responsible for governance authority must demonstrate **documented competence appropriate to system risk classification**.

Governance authority without demonstrable competence is prohibited.

---

### Vendor-Triggered Governance Controls

Vendor-driven model updates or integration changes meeting the definition of **Materially Affecting Behavior** must:

- undergo evaluation  
- receive documented authorization  
- trigger operational review  
- remain traceable within governance artifacts  

Delegation to vendors does **not** transfer governance accountability.

---

### Oversight vs Monitoring

DAGS distinguishes between:

- **operational monitoring mechanisms**
- **independent governance oversight authority**

Monitoring supports oversight but does not substitute for it.

---

### Reconstruction and Traceability

Governance artifacts must support reconstruction of system operation including:

- output  
- timestamp  
- model version  
- configuration state  
- authorization record  
- affected party where applicable  

Reconstruction must not rely on informal recollection or vendor-only artifacts.

---

## Compatibility

Version **1.1** is fully **backward compatible with v1.0**.

Organizations previously assessed against v1.0 are not rendered non-compliant by the additions introduced in v1.1.

Deployers operating agentic or multi-system execution environments should evaluate applicability of controls **D3.19–D3.32** within their operational context.

---

## Cross-Domain Integration

The cross-domain architecture established in **v1.0** remains unchanged.

The standard continues to operate across the following domains:

- **D1 — Governance and Accountability**  
- **D2 — Model and Vendor Visibility**  
- **D3 — Security and Controls**  
- **D4 — Ethics and Responsible Use**  
- **D5 — Operational Integration**

The doctrine of **Materiality** continues to operate as a cross-domain governance principle.

---

## Forward-Looking Notes

Future revisions may include:

- methodologies for determining materiality in agentic environments  
- implementation guidance for execution path identifiers  
- cross-system log correlation guidance  
- expanded alignment references to external regulatory frameworks  
- assessment instruments for controls **D3.19–D3.32**

Such additions would not alter the **normative requirements of v1.1**.
