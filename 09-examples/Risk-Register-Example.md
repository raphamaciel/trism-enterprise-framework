# Example Risk Register (Fictional)

This example is fictional and for learning purposes only. Adapt fields, scoring, and treatment plans to your organization.
This example is not legal advice, not a certification artifact, and not a compliance guarantee.

| Risk ID | Domain | Description | Likelihood (1-5) | Impact (1-5) | Inherent Score | Treatment Strategy | Risk Owner | Review Cadence | Due Date | Residual Score | Risk Status |
|---|---|---|---|---|---|---|---|---|---|---|---|
| RSK-001 | Security | Prompt injection can trigger unsafe tool calls in agent workflow. | 4 | 5 | 20 | Reduce | Security Engineering Lead | Monthly | 2026-05-15 | 8 | Open |
| RSK-002 | Privacy | Sensitive customer data may appear in model outputs due to retrieval misconfiguration. | 3 | 5 | 15 | Reduce | Privacy Lead | Monthly | 2026-05-30 | 6 | Open |
| RSK-003 | Model Risk | Performance drift in regional traffic leads to degraded recommendation quality. | 3 | 4 | 12 | Reduce | Model Risk Lead | Monthly | 2026-06-10 | 5 | Mitigated |
| RSK-004 | Governance | Gate approvals bypassed during emergency release process. | 2 | 5 | 10 | Avoid | Governance Lead | Quarterly | 2026-05-05 | 3 | Accepted |

## Notes
- Inherent Score formula example: Likelihood x Impact.
- Residual score should be recalculated after controls are implemented.
- Accepted risks should include approval, rationale, and review date in decision logs.
