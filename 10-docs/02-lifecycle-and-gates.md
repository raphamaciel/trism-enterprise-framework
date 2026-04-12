# Lifecycle and Gates Guide

## Purpose
Explain where each governance gate applies and which repository artifacts support that gate.

## Lifecycle Phases
- Design
- Deployment
- Runtime operations
- Audit and review

## Canonical Gates
| Gate | Name | Primary Objective | Typical Exit Criteria |
|---|---|---|---|
| Gate 1 | Design Assurance | Confirm architecture, threat model, and control intent | Threat model complete, control mapping drafted, design decisions documented |
| Gate 2 | Pre-Production Assurance | Confirm test evidence and risk treatment readiness | Risk register updated, model and system assurance evidence attached, security and privacy evidence linked |
| Gate 3 | Go-Live Assurance | Confirm production authorization | High and critical findings resolved or accepted, approvals complete, incident readiness validated |
| Gate 4 | Post-Live Assurance | Confirm ongoing runtime governance | Monitoring active, drift and abuse alerts active, recurring reviews scheduled |

## Folder-to-Lifecycle Mapping
| Folder | Lifecycle Focus | Main Outputs |
|---|---|---|
| 01-governance | Cross-cutting | charter, control mappings, impact assessments |
| 02-architecture-threat-modeling | Design | system and AI-specific threat models |
| 03-risk-control-registers | Design to runtime | risk identification and treatment tracking |
| 04-model-assurance | Pre-production and runtime | model and system assurance evidence |
| 05-security-privacy-evidence | Pre-production and runtime | security, privacy, and monitoring evidence |
| 06-deployment-gates | Deployment | gate checklists and approval records |
| 07-audit-evidence-decisions | Audit and review | decision logs, exceptions, sensitive use reviews |
| 08-agents | Design to runtime | agent specifications and governance controls |
| 09-examples | Learning support | fictional reference artifacts |
| 99-operations | Runtime and review | incident response and feedback loop documentation |

## Gate Execution Checklist
1. Confirm target gate and release scope.
2. Attach required artifacts and evidence links.
3. Validate ownership and review dates.
4. Route PR to required approvers.
5. Record decision and any exceptions.

## Sources
- SRC-NIST-001
- SRC-GARTNER-001

Last verified: 2026-04-12
