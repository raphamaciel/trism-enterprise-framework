# Deployment Gate Naming Standard

## Purpose
Define canonical gate names and terms for consistent use across repository artifacts.

## Canonical Gates
| Gate ID | Canonical Name | Lifecycle Stage | Primary Objective |
|---|---|---|---|
| Gate 1 | Design Assurance | Design | Confirm architecture, threat model, and control intent before build progression |
| Gate 2 | Pre-Production Assurance | Pre-production | Confirm test evidence, risk treatments, and control readiness before production approval |
| Gate 3 | Go-Live Assurance | Release | Confirm production authorization based on complete evidence and approvals |
| Gate 4 | Post-Live Assurance | Runtime operations | Confirm ongoing monitoring, drift handling, and review cadence after release |

## Terminology Rules
- Always reference gates as "Gate N: Canonical Name".
- Do not rename gates across teams or artifacts.
- Use the same gate names in pull requests, approvals, and audit logs.

## Required Usage Locations
- Deployment gate checklist
- Pull request gate template
- Governance checklist
- Decision and exception logs
