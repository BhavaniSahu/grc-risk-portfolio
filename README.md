# GRC Risk & Compliance Portfolio

A working portfolio of GRC analysis built during a self-directed technical study program, demonstrating the ability to take a technical finding through the full compliance lifecycle: threat modeling, risk quantification, multi-framework control mapping, and plain-language stakeholder communication.

**All findings in this repository are hypothetical/generalized examples built for training purposes. Nothing here describes any employer's real environment, systems, or data.**

## What's here

| File | Contents |
|---|---|
| [`01-risk-register.md`](01-risk-register.md) | Vulnerability-to-control mapping: inherent/residual risk, ISO/IEC 27001 controls, NIST CSF 2.0 subcategories, India DPDP Act, 2023 sections, and a plain-English business translation for each finding |
| [`02-stride-threat-model.md`](02-stride-threat-model.md) | Per-finding STRIDE threat modeling (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege) with applicability, existing controls, and residual exposure |
| [`03-risk-treatment-ale.md`](03-risk-treatment-ale.md) | Risk treatment decisions (Mitigate/Accept/Transfer/Avoid) backed by quantitative Annualized Loss Expectancy (ALE) modeling |
| [`04-framework-reference.md`](04-framework-reference.md) | Reusable reference material: risk rating scale, STRIDE definitions, ISO/IEC 27001 clause structure, NIST CSF 2.0 category map |

## Frameworks applied

- **ISO/IEC 27001** — Annex A controls and Clause 4-10 management system requirements
- **NIST CSF 2.0** — Govern / Identify / Protect / Detect / Respond / Recover functions
- **India's Digital Personal Data Protection (DPDP) Act, 2023**
- **STRIDE** threat modeling methodology
- **Quantitative risk analysis** (SLE / ARO / ALE)

## Why this exists

Technical findings only create value once they're translated into a form auditors, risk committees, and business stakeholders can act on. Each entry in the risk register pairs the technical detail with a control mapping across three frameworks and a business-language explanation — the same translation exercise used in live control walkthroughs and audit interviews.
