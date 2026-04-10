# TRiSM Agents

This folder defines core operational agents used by the TRiSM framework.

This repository is an independent, experimental governance-as-code project. It is not affiliated with or endorsed by Gartner and does not provide certification, legal advice, or compliance guarantees.

Agent specifications are templates and examples that require organization-specific adaptation.

## Folder Structure
- One folder per agent using pattern: `AGT-<id>-<slug>/`
- Each agent folder contains:
	- `agent.md` for the primary agent specification
	- `skills/` for future agent-specific skills and assets
- Shared templates and reusable assets are under `shared/`

## Agent Set

### TRiSM Core Agents
- AGT-001 Deployment Gatekeeper Agent
- AGT-002 Control Evidence Agent
- AGT-003 Model Risk Assessment Agent
- AGT-004 Runtime Monitoring and Drift Agent

### Microsoft Responsible AI Standard (RAS) Agents
- AGT-005 AI Impact Assessment Agent
- AGT-006 Fairness and Inclusiveness Monitoring Agent
- AGT-007 Sensitive Use Triage Agent

## Common Contract

Each agent specification includes:
- mission and scope
- required inputs and upstream dependencies
- outputs and generated artifacts
- escalation and human approval boundaries
- KPI and KRI measures
- integration points with repository templates
- governance controls for allowed actions, autonomy, and shutdown behavior

## Implementation Notes

- All high-risk decisions require human approval.
- All agent actions must produce immutable decision logs.
- Agent outputs should be attached to pull requests for auditability.
- Use `shared/templates/Agent-Governance-Control-Template.md` for agent-level control design and revalidation.
