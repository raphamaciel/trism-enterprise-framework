# Artifact Usage Guide

## Purpose
Help contributors understand when to use each artifact template, who should own it, and what minimum fields are required.

## Usage Matrix
| Artifact Area | When to Use | Primary Owner | Minimum Completion Criteria |
|---|---|---|---|
| Governance charter and mappings | Initial setup and quarterly reviews | Governance Lead | Scope, owners, review cadence, approved policy mapping |
| Threat modeling templates | New systems and major design changes | Security Lead | Threat scenarios, controls, residual risk, approvals |
| Risk register template | Every release cycle | Risk Owner | Likelihood, impact, treatment, owner, status, review cadence |
| Model and system assurance templates | Before Gate 3 and during monitoring updates | Model Risk Lead and Platform Lead | Metrics, thresholds, limitations, approvals |
| Security and privacy evidence template | Before Gate 3 and monthly review | Security Lead and Privacy Lead | Control validation evidence and runtime monitoring evidence |
| Gate checklist template | Each release decision | Governance Lead and Platform Lead | Required checks complete and decision record populated |
| Decision and exception templates | Any exception or high-impact decision | Governance Lead | Owner, justification, review criteria, review date |
| Agent governance templates | For each agent specification and updates | Agent Owner | Allowed actions, autonomy level, human review, shutdown rules |
| Operations feedback loop docs | Incident and post-incident follow-up | Incident Commander and Governance Lead | Incident record, control update, verification evidence |

## Common Mistakes to Avoid
- Submitting artifacts without named owners.
- Marking risks as accepted without review criteria.
- Linking frameworks as if they imply certification.
- Using examples as production-ready artifacts without adaptation.

## Suggested Contributor Path
1. Read docs/01-concepts.md.
2. Read docs/02-lifecycle-and-gates.md.
3. Select and complete required templates.
4. Open PR using the governance template.
5. Obtain approvals and record the decision.

## Example References
- 09-examples/Risk-Register-Example.md
- 09-examples/Model-Card-Example.md
- 09-examples/Deployment-Gate-Approval-Example.md
