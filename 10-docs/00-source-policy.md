# Source and Citation Policy

## Purpose
Define how factual claims are sourced, reviewed, and maintained in this repository.

## Positioning
This repository is an independent, experimental governance-as-code project. It is not affiliated with or endorsed by Gartner and does not provide certification, legal advice, or compliance guarantees.

## Source Tiers
| Tier | Type | Examples | Usage Rule |
|---|---|---|---|
| Tier 1 | Primary official sources | NIST, EUR-Lex, OECD, official Microsoft and Google responsible AI pages | Preferred for normative statements |
| Tier 2 | Official secondary sources | Government guidance pages, standards body summaries | Use when full primary text is unavailable |
| Tier 3 | Commentary and analysis | Vendor blogs, analyst commentary, educational articles | Use for context only, not normative claims |

## Citation Rules
1. Use a source identifier from `10-docs/11-reference-register.md` for factual or normative statements.
2. If a statement includes language such as "must", "required", or "obligation", include at least one Tier 1 or Tier 2 source.
3. Separate facts from implementation interpretation.
4. Add a "Last verified" date for every framework deep-dive page.

## Writing Pattern
For major statements, use this pattern:
- Fact: What the source says.
- Interpretation: How this repository applies it.
- Source ID: One or more IDs from the reference register.

## Prohibited Claim Pattern
Do not write claims implying:
- endorsement or sponsorship by Gartner
- formal certification status
- guaranteed compliance outcomes

## Review Cadence
- Source links: quarterly verification
- High-impact framework pages: monthly verification
- Regulatory pages: verify after major legal updates

## Sources
- SRC-NIST-001
- SRC-EU-001
- SRC-OECD-001
- SRC-MS-001
- SRC-GOOG-001
- SRC-ISO-001

Last verified: 2026-04-12
