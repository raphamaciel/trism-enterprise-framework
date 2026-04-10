# Incident to Control Feedback Loop

## Purpose
Define an explicit operational loop that converts production incidents into governance and control improvements.

## Loop Stages
1. Incident Detection
2. Incident Triage and Containment
3. Root Cause and Governance Review
4. Control Update and Approval
5. Verification and Closure

## Operating Procedure

### 1. Incident Detection
- Source: monitoring alerts, user reports, red team tests, audit findings.
- Output: incident ticket with severity and owner.

### 2. Incident Triage and Containment
- Classify severity and affected scope.
- Apply containment actions for user and system safety.
- Log emergency decisions in decision register.

### 3. Root Cause and Governance Review
- Determine whether failure was control design, implementation, operation, or oversight.
- Identify which gate and control set failed or was bypassed.

### 4. Control Update and Approval
- Update relevant artifacts:
  - control matrix
  - risk register
  - threat model
  - gate checklist
  - agent governance controls
- Route changes through pull request review and required approvals.

### 5. Verification and Closure
- Verify updated controls in test and runtime telemetry.
- Record closure criteria and evidence links.
- Schedule follow-up review for recurrence prevention.

## Metrics
- Mean time from incident to control update
- Percentage of incidents with completed governance review
- Recurrence rate for same incident category

## Ownership
- Incident Commander: operational response
- Governance Lead: control and policy updates
- Platform Lead: technical remediation
- Risk Owner: risk register updates
