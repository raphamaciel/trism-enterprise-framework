# AGT-002 Control Evidence Agent

## Mission
Continuously collect, validate, and attach objective evidence for each TRiSM control.

## Scope
- Control evidence freshness
- Evidence traceability to specific control IDs
- Release-level evidence bundle generation

## Inputs
- Control matrix from 01-governance
- CI/CD pipeline logs and build attestations
- Security scan outputs
- Model evaluation reports
- Approval and exception records

## Decision Policy
- Mark control as At Risk if evidence is stale beyond configured SLA.
- Mark control as Failed if no valid evidence exists for a required gate.
- Mark control as Passing only when evidence is current, complete, and linked.

## Outputs
- Control evidence status table by control ID.
- Release evidence bundle with immutable references.
- Evidence gap report for unresolved controls.

## Human Approval Boundary
- Internal Audit Liaison validates periodic evidence completeness.
- Governance Lead approves evidence waivers.

## Escalation
1. Control owner
2. Internal Audit Liaison
3. AI Governance Lead

## KPIs
- Percentage of controls with current evidence
- Evidence generation cycle time
- Audit request response time

## KRIs
- Number of controls missing evidence at release time
- Number of stale evidence artifacts above SLA

## Repository Artifacts
- Uses 01-governance/Control-Matrix-Template.md
- Updates 07-audit-evidence-decisions/Decision-Log-Template.md
