# Review and Approval Workflow

## Purpose
Define an auditable, repeatable review and approval process for governance artifacts and release gates.

## Workflow Summary
1. Artifact Preparation
2. Pull Request Submission
3. Evidence and Control Validation
4. Role-Based Review and Decision
5. Merge, Record, and Post-Decision Follow-Up

## Detailed Process

### 1. Artifact Preparation
- Populate required templates for target lifecycle stage.
- Assign owners and review cadence.
- Link evidence artifacts and source references.

### 2. Pull Request Submission
- Use `.github/PULL_REQUEST_TEMPLATE/trism-gate.md`.
- Identify target gate and impacted controls.
- Attach required evidence links.

### 3. Evidence and Control Validation
- Validate gate checklist completeness.
- Validate decision and exception traceability fields.
- Validate positioning and claims policy adherence.
- Validate documentation source metadata via CI.

### 4. Role-Based Review and Decision
- Governance Lead: gate decision owner.
- Security Lead: security control sign-off.
- Privacy Lead: privacy impact sign-off.
- Model Risk Lead: model/system assurance sign-off.
- Platform Lead: release readiness sign-off.

Decision outcomes:
- Approved
- Conditional approval with explicit conditions
- Rejected with remediation actions

### 5. Merge, Record, and Follow-Up
- Merge only after required approvals and passing checks.
- Update decision and exception artifacts.
- Schedule follow-up review based on decision conditions.

## Minimum Required Evidence by Gate
| Gate | Required Minimum Evidence |
|---|---|
| Gate 1: Design Assurance | Threat model, initial control mapping, architecture decision context |
| Gate 2: Pre-Production Assurance | Risk register updates, model and system assurance evidence, security/privacy evidence |
| Gate 3: Go-Live Assurance | Approver sign-offs, open-finding dispositions, incident readiness evidence |
| Gate 4: Post-Live Assurance | Monitoring evidence, drift and abuse controls, recurring review schedule |

## Escalation Rules
- Critical unresolved findings at Gate 3 should block release unless formally accepted with compensating controls.
- Expired exceptions should trigger escalation before merge.
- Repeated incidents in same category should trigger control update review.

## Sources
- SRC-NIST-001
- SRC-NIST-002
- SRC-EU-001
- SRC-MS-001
- SRC-GOOG-001

Last verified: 2026-04-12
