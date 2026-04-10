# Example Model Card (Fictional)

This model card is fictional and intended to demonstrate how assurance artifacts can be populated.
This example is not legal advice, not a certification artifact, and not a compliance guarantee.

## Model Identity
- Model name: SupportCaseAssist-v2
- Version: 2.3.1
- Owner: AI Platform Team
- Intended use: Draft response suggestions for internal support analysts.
- Out-of-scope use: Automated customer-facing final decisions without human review.

## Training and Data Overview
- Data sources: Historical support tickets, curated knowledge base, policy documents.
- Data limitations: Underrepresentation of low-volume product lines in training corpus.
- Sensitive attribute handling: Sensitive attributes excluded from feature set and masked in logs.

## Performance and Quality
| Metric | Segment | Baseline | Current | Threshold | Status |
|---|---|---|---|---|---|
| Accuracy | Global | 0.88 | 0.90 | >= 0.86 | Pass |
| Accuracy | APAC | 0.85 | 0.84 | >= 0.83 | Pass |
| Hallucination rate | Global | 0.08 | 0.06 | <= 0.07 | Pass |
| Response latency (p95) | Global | 1700 ms | 1550 ms | <= 1800 ms | Pass |

## Risk and Safety
- Bias and fairness assessment summary: No severe disparity detected in quality metrics across tested regions and language groups.
- Robustness and adversarial testing summary: Prompt injection defenses blocked 92 percent of known attack prompts in staging tests.
- Explainability method used: Retrieved evidence snippets and confidence band shown to reviewer.

## Monitoring
- Drift indicators: Embedding distribution shift, intent classification drift, and retrieval mismatch rate.
- Alert thresholds: Drift warning > 0.15 PSI, critical > 0.25 PSI.
- Rollback criteria: Two consecutive critical drift events or severe incident classification.

## Approval
- Model Risk Lead: Approved with monthly drift review condition
- Governance Lead: Approved for controlled production rollout
