# Framework Deep Dive: NIST AI RMF

## Purpose
Summarize NIST AI RMF in operational terms and show how repository artifacts can align with it.

## What It Is
NIST AI RMF is a voluntary risk management framework for AI systems organized around four functions: Govern, Map, Measure, and Manage.

## Scope and Applicability
- Applicable across AI lifecycle phases.
- Useful for governance design, risk process definition, and measurement discipline.
- Not a certification mechanism.

## Fact vs Interpretation
| Type | Statement | Source ID | Confidence |
|---|---|---|---|
| Fact | AI RMF is structured into Govern, Map, Measure, Manage functions. | SRC-NIST-001 | High |
| Fact | NIST provides a playbook to support implementation examples and actions. | SRC-NIST-002 | High |
| Interpretation | Repository gates and evidence workflows can be used as implementation mechanisms for RMF-aligned controls. | SRC-NIST-001, SRC-NIST-002 | Medium |

## Practical Mapping in This Repository
- Govern: `01-governance`, `07-audit-evidence-decisions`
- Map: `02-architecture-threat-modeling`, `03-risk-control-registers`
- Measure: `04-model-assurance`, `05-security-privacy-evidence`
- Manage: `06-deployment-gates`, `99-operations`

## What It Does Not Provide
- Legal compliance determination
- Product-specific implementation details by default

## Sources
- SRC-NIST-001
- SRC-NIST-002

Last verified: 2026-04-12
