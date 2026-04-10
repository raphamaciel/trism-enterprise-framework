# Enterprise TRiSM Artifact Repository

This is an AI generated repository to provide a practical Governance-as-Code structure for Trust, Risk, and Security Management (TRiSM) in enterprise framework deployments.

## Purpose

- Standardize TRiSM artifacts across design, deployment, and operations.
- Create auditable evidence for approvals and regulatory reviews.
- Enforce deployment gates based on trust, risk, and security controls.

## Repository Structure

- `01-governance` - policy, governance charter, and control mapping
- `02-architecture-threat-modeling` - system context and threat models
- `03-risk-control-registers` - risk register and treatment tracking
- `04-model-assurance` - model cards and validation reports
- `05-security-privacy-evidence` - security baseline and privacy impact evidence
- `06-deployment-gates` - gate checklists and approval records
- `07-audit-evidence-decisions` - exception logs and decision records
- `08-agents` - operational agent specifications and catalog
- `99-operations` - runbooks, KPI/KRI dashboards, and review cadence

## How To Use

1. Copy templates and create versioned artifacts per deployment release.
2. Open a pull request using `.github/PULL_REQUEST_TEMPLATE/trism-gate.md`.
3. Complete the governance checklist in `.github/trism-governance-checklist.md`.
4. Route approvals to required reviewers before merge.

## Governance Cadence

- Monthly: risk and monitoring review
- Quarterly: control and policy review
- Per release: Gate 1 through Gate 4 evidence check

## Suggested Next Steps

1. Initialize git and push:
   - `git init`
   - `git add .`
   - `git commit -m "Initial TRiSM governance repository scaffold"`
2. Create GitHub branch protections on `main`.
3. Configure required reviewers for risk, security, privacy, and platform leads.

## 🧠 AI Governance Frameworks — Executive Comparison

> **One framework is not enough.**  
> Effective AI governance combines ethics, risk management, regulation, engineering practices, and runtime controls.

| Framework | Primary Purpose | Focus Level | Best At | Key Limitation |
| --- | --- | --- | --- | --- |
| **OECD AI Principles** | Ethics & trust | Values & policy | Establishing **global norms** for trustworthy, human‑centric AI | Non‑operational |
| **NIST AI Risk Management Framework (RMF)** | AI risk management | Lifecycle & risk | Structuring AI risk via **Govern · Map · Measure · Manage** | Limited runtime enforcement |
| **ISO/IEC 42001** | Enterprise AI governance | Organisation & process | **Certifiable AI management system** for board‑level assurance | Governance‑heavy, not technical |
| **EU AI Act** | Regulation & compliance | Legal | **Mandatory, risk‑based obligations** with enforcement | Defines *what*, not *how* |
| **Microsoft Responsible AI Standard** | Engineering governance | Product & platform | **Practical engineering controls** embedded into AI development | Vendor‑specific |
| **Google Responsible AI** | Safety & research practices | Model & tooling | Advanced **safety testing, red‑teaming, and transparency** | Not enterprise‑wide governance |
| **Gartner AI TRiSM** | Trust, risk & security | **Runtime & enforcement** | **Continuous monitoring and guardrails** for AI in production | Emerging, multi‑tool market |

---

### ✅ Executive takeaway

**Modern AI governance requires a layered approach:**

- **Principles** → OECD AI Principles  
- **Risk management** → NIST AI RMF  
- **Organisational governance & assurance** → ISO/IEC 42001  
- **Regulatory compliance** → EU AI Act  
- **Engineering practices** → Microsoft & Google Responsible AI  
- **Runtime trust & control** → **Gartner AI TRiSM**

> **TRiSM is the missing operational layer** — ensuring AI behaves safely *after deployment*, not just at design time.

## Sources & references
- https://www.gartner.com/en/articles/ai-trust-and-ai-risk
- https://www.ibm.com/think/topics/ai-trism
- https://transcend.io/blog/ai-trism
- https://education.securiti.ai/certifications/ai-governance/introduction-to-ai-governance/ai-trism/
- https://www.skillsoft.com/course/emerging-data-trends-ai-trism-unleashed-60efb41f-1b9c-40b9-b1fa-d5dcdb006e58
