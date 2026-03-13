# Changelog

All notable changes to the Deployment AI Governance Standard (DAGS) are documented in this file.

This project follows the Keep a Changelog format adapted for governance standards.

## v1.1 — 2026-03-11

**Status:** Published

**Normative Status:** Additive Minor Release

**Supersedes:** v1.0

## Summary

Version 1.1 extends the Deployment AI Governance Standard to address agentic deployment environments in which AI-enabled systems initiate and propagate consequential actions across multiple systems, services, and tools.

The five-domain architecture remains unchanged.

All controls introduced in v1.0 (D1.1–D5.13) remain in force without modification.

Version 1.1 introduces 14 new controls within Domain D3, increasing the total number of normative controls from 57 to 71.

## Normative Additions

### Domain D3 — Security and Controls

#### Authority Continuity Controls

D3.19 – D3.22

These controls govern preservation and enforcement of authorization constraints across execution paths spanning multiple systems.

Key governance requirements include:
- preservation of original authorization scope
- prohibition of implicit privilege expansion
- revalidation of authority during propagation
- independent enforcement across system boundaries

#### Identity and Delegation Controls

D3.23 – D3.26

These controls govern identity propagation and delegation integrity across execution paths.

Key governance requirements include:
- privilege scoping across delegated actions
- credential propagation constraints
- identity provenance verification
- prevention of scope expansion during delegation.

#### Execution Path Evidence Controls

D3.27 – D3.32

These controls establish evidence standards for reconstruction of agentic execution paths.

Required governance artifacts include:
- persistent execution path identifiers
- authority lineage records
- materiality threshold snapshots
- irreversibility markers
- chain terminal records.

Execution path governance applies only to operations capable of producing consequential state change.

## Normative Terminology Additions

Version 1.1 introduces five defined terms governing agentic execution governance:
- Execution Path
- Execution Path Initiation Event
- Legibility Boundary
- Planning Authority
- Materiality Threshold

These terms clarify governance obligations when authorized actions propagate across multiple systems or agents.

## Structural Clarifications

The following governance doctrines introduced in v1.0 remain in force and unchanged in v1.1.

### Materially Affecting Behavior

The defined term Materially Affecting Behavior governs:
- change authorization thresholds
- vendor update triggers
- logging requirements
- reconstruction obligations
- ethical oversight escalation.

Materiality determinations must be documented, attributable, and periodically reassessed.

### Strategy vs Deployment Boundary

DAGS governs the deployment layer of AI systems, not organizational AI strategy.

However, enterprise strategy and ethical commitments define the accountability perimeter within which deployment governance operates.

### Operationalization of Ethical Constraints

Ethical commitments must be translated into enforceable operational controls including:
- transparency of system purpose and limitations
- explainability appropriate to system risk
- fairness and non-discrimination safeguards
- performance monitoring
- human oversight capability.

Aspirational ethical statements without enforceable controls are insufficient.

### Governance Competence Requirement

Individuals responsible for governance authority must demonstrate documented competence appropriate to system risk classification.

Governance authority without demonstrable competence is prohibited.

### Vendor-Triggered Governance Controls

Vendor-driven model updates or integration changes meeting the definition of materially affecting behavior must:
- undergo evaluation
- receive documented authorization
- trigger operational review
- remain traceable within governance artifacts.

Delegation to vendors does not transfer governance accountability.

### Oversight vs Monitoring

DAGS distinguishes between:
- operational monitoring
- independent governance oversight authority

Monitoring supports oversight but does not substitute for it.

### Reconstruction and Traceability

Governance artifacts must support reconstruction of system operation including:
- output
- timestamp
- model version
- configuration state
- authorization record
- affected party where applicable.

Reconstruction must not rely on informal recollection or vendor-only artifacts.

## Compatibility

Version 1.1 is backward compatible with v1.0.

Organizations assessed against v1.0 are not rendered non-compliant by the v1.1 additions alone. Deployers operating agentic systems should evaluate applicability of controls D3.19–D3.32 within their operational environment.

## Cross-Domain Integration

The cross-domain architecture established in v1.0 remains unchanged.

D1 — Governance and Accountability

D2 — Model and Vendor Visibility

D3 — Security and Controls

D4 — Ethics and Responsible Use

D5 — Operational Integration

Materiality operates as a cross-domain doctrine spanning all domains.

## Forward-Looking Notes

Future revisions may include:
- materiality determination methodologies for agentic environments
- execution path identifier implementation guidance
- cross-system log correlation guidance
- expanded regulatory alignment references
- assessment instruments for new D3 controls.

These additions would not alter the normative requirements of v1.1.
