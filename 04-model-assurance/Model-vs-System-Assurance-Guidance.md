# Model vs System Assurance Guidance

## Purpose
Clarify the difference between model-level assurance and system-level assurance for AI systems, including GenAI pipelines.

## Model Assurance
Model assurance validates behavior of the model artifact itself.

Typical scope:
- Model quality and performance metrics
- Fairness and bias evaluation
- Robustness and adversarial resilience
- Explainability and limitations
- Drift indicators tied to model behavior

Primary artifacts:
- Model card
- Fairness evaluation report
- Safety evaluation report

## System Assurance
System assurance validates the end-to-end AI solution in its deployed operating context.

Typical scope:
- Prompt and retrieval pipeline behavior
- Agent tool usage and action boundaries
- Access controls and secrets handling
- Runtime monitoring and abuse detection
- Human oversight and escalation flow

Primary artifacts:
- Threat model
- Deployment gate records
- Security and privacy evidence
- Incident response playbook

## GenAI Pipeline Note
For GenAI and agentic systems, model assurance alone is insufficient.

Production assurance should evaluate the full chain:
User input -> Prompt processing -> Retrieval and context -> Model output -> Agent actions -> Human review and controls.

## Review Requirement
Both model and system assurance evidence should be attached before Gate 3 Go-Live Assurance.
