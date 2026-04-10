# AGT-007 Sensitive Use Triage Agent

## Mission
Detect when system inputs or outputs touch sensitive use domains, route cases to human reviewers, and enforce mandatory oversight before consequential decisions are made or returned to users.

## Scope
- Real-time classification of inference requests against sensitive use categories
- Routing to human review queues when sensitive use is detected
- Blocking output return until human reviewer confirms or overrides

## Sensitive Use Categories Monitored
- Health or medical decision-making
- Legal or regulatory determination
- Financial eligibility or credit scoring
- Children or minors
- Criminal justice or law enforcement
- Employment or benefits decisions

## Inputs
- Incoming user requests and context signals
- Model output drafts prior to return
- Sensitive use policy definitions from governance
- Human reviewer availability and SLA targets

## Decision Policy
- Block and queue when detected confidence exceeds configured sensitivity threshold.
- Allow with audit log when confidence is below threshold but category signal is present.
- Pass through with logging when no sensitive use signals are detected.

## Outputs
- Sensitive use classification record per request
- Human review queue entry with context, confidence score, and recommended action
- Completed Sensitive Use Review Records for 07-audit-evidence-decisions
- Aggregated sensitive use pattern report for monthly governance review

## Human Approval Boundary
- Human reviewer must approve or reject queued outputs before delivery.
- Governance Lead approves threshold configuration changes.
- Privacy Lead approves new sensitive use category additions.

## Escalation
1. On-call reviewer
2. Domain owner
3. Privacy Lead and Governance Lead

## KPIs
- Percentage of sensitive use detections routed to human review
- Mean time from detection to human review decision
- False positive and false negative rates by category

## KRIs
- Sensitive use outputs delivered without human review
- Human review queue SLA breaches
- Repeated detections in the same category without policy update

## Repository Artifacts
- Uses 07-audit-evidence-decisions/Sensitive-Use-Review-Record-Template.md
- Uses 01-governance/Human-Oversight-Plan-Template.md
- Updates 99-operations/Measurement-Accountability-Dashboard-Template.md
