# Role-Based Playbooks

## Purpose
Provide practical role-specific execution steps for using repository artifacts in real governance workflows.

## Positioning
This repository is an independent, experimental governance-as-code project. It is not affiliated with or endorsed by Gartner and does not provide certification, legal advice, or compliance guarantees.

## Governance Lead Playbook
### Inputs
- 01-governance artifacts
- 06-deployment-gates checklists
- 07-audit-evidence-decisions records

### Steps
1. Confirm release scope and target gate.
2. Verify control ownership and review cadence.
3. Confirm required evidence is linked in PR.
4. Validate exception records include owner, expiry, and review criteria.
5. Issue approval, conditional approval, or rejection with rationale.

### Outputs
- Gate decision
- Updated decision log
- Updated exception register where applicable

## Security Lead Playbook
### Inputs
- Threat model artifacts
- Security evidence and findings
- Runtime abuse and anomaly signals

### Steps
1. Review threat scenarios and control coverage.
2. Validate open findings disposition and due dates.
3. Confirm minimum runtime controls are active.
4. Sign off or request mitigation conditions.

### Outputs
- Security sign-off record
- Security exceptions and compensating controls

## Privacy Lead Playbook
### Inputs
- DPIA and privacy evidence
- Sensitive use review records
- Data handling and retention controls

### Steps
1. Confirm legal basis and privacy impact treatment.
2. Validate rights and retention controls are documented.
3. Verify sensitive-use routing and oversight requirements.
4. Approve or escalate based on residual privacy risk.

### Outputs
- Privacy sign-off
- Privacy risk treatment actions

## Model Risk Lead Playbook
### Inputs
- Model and system assurance artifacts
- Fairness and safety evaluations
- Drift thresholds and monitoring setup

### Steps
1. Verify performance and safety thresholds.
2. Validate fairness and explainability evidence.
3. Review drift and rollback criteria.
4. Approve, conditionally approve, or block release.

### Outputs
- Model risk decision
- Required remediation list

## Platform Engineering Lead Playbook
### Inputs
- Gate checklists
- CI/CD validation outputs
- Runtime monitoring and incident readiness

### Steps
1. Confirm gate controls are enforceable in pipeline.
2. Validate deployment and rollback readiness.
3. Confirm alerting and on-call ownership.
4. Apply go-live action after all required approvals.

### Outputs
- Deployment authorization record
- Runtime readiness confirmation

## Internal Audit Liaison Playbook
### Inputs
- Decision logs
- Exception register
- Evidence links

### Steps
1. Verify traceability from control to evidence.
2. Confirm exceptions are time-bound and owned.
3. Validate periodic review execution against cadence.
4. Record findings for governance review.

### Outputs
- Audit readiness assessment
- Follow-up recommendations

## Sources
- SRC-NIST-001
- SRC-NIST-002
- SRC-EU-001
- SRC-MS-001
- SRC-GOOG-001
- SRC-OECD-001
- SRC-GARTNER-001

Last verified: 2026-04-12
