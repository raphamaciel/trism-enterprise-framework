# Example Deployment Gate Approval (Fictional)

This approval record is fictional and demonstrates a practical Gate 3 decision entry.

## Gate Context
- Gate: Gate 3: Go-Live Assurance
- Release ID: rel-2026-04-10-rc2
- Environment: Production
- Change scope: Enable agent-assisted response drafting for Tier 1 support queue

## Evidence Summary
- Threat model updated and approved: Yes
- Risk register updated with owners and treatment dates: Yes
- Model assurance and system assurance attached: Yes
- Security and privacy evidence attached: Yes
- Sensitive use review required: No

## Open Findings Review
| Finding ID | Severity | Disposition | Owner | Due Date |
|---|---|---|---|---|
| FND-114 | Medium | Accepted with compensating control | Security Lead | 2026-05-01 |
| FND-121 | Low | Scheduled remediation | Platform Lead | 2026-04-25 |

## Decision
- Decision: Conditional Approval
- Justification: Mandatory controls are met for go-live. One medium finding has approved compensating control and documented expiry.
- Conditions:
  1. Weekly drift report to Governance Lead for first 30 days.
  2. Complete FND-114 remediation by due date or trigger rollback review.
- Review criteria: If drift exceeds critical threshold twice in 14 days, initiate incident response and suspend rollout.
- Next review date: 2026-05-10

## Approvers
- AI Governance Lead: Approved
- Security Lead: Approved
- Privacy Lead: Approved
- Model Risk Lead: Approved
- Platform Engineering Lead: Approved
- Date: 2026-04-10
