# Framework Reference

Reusable lookup material: risk rating scale, STRIDE category definitions, ISO/IEC 27001 clause & control structure, and the NIST CSF 2.0 category map.

## Risk Rating Scale

| Rating | Likelihood Guidance | Impact Guidance | Typical Action |
|---|---|---|---|
| Critical | Actively exploited in the wild / trivial to exploit, no barriers | Regulatory breach, major financial loss, business-stopping | Remediate immediately, escalate to leadership same day |
| High | Exploitable with moderate skill, exposed to untrusted network | Significant data exposure or service disruption | Remediate within days, track at risk committee |
| Medium | Requires specific conditions or insider access | Limited data exposure, contained disruption | Remediate within a defined SLA (e.g. 30-90 days) |
| Low | Theoretical or requires extensive prerequisites | Minimal or no material impact | Track and accept, or fix opportunistically |

## STRIDE Category Definitions (sample)

| STRIDE Category | Property Violated | Test / Notes |
|---|---|---|
| Spoofing | Authentication | Can someone pretend to be someone/something they're not? |  |
| Information Disclosure | Confidentiality | Does access match authorization -- not just 'is the content sensitive'. Unauthorized READ access is disclosure on its own, regardless of content; sensitive content increases severity but doesn't gate whether the category applies. Covers external leaks, over-broad access for authenticated users (IDOR-style), and side channels (error messages, timing). |  |

*(Full six-category breakdown — Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege — is applied per-finding in `02-stride-threat-model.md`.)*

## ISO/IEC 27001 Clauses (4-10) — Memory Aid

Story: *"Know your world (4), get leaders on board (5), make a plan (6), get support (7), run it (8), check it (9), fix it (10)"* — this mirrors the PDCA cycle.

| Clause | Name | PDCA Stage | Memory Peg |
|---|---|---|---|
| 4 | Context of the Organization | Plan | Know your world - internal/external issues, interested parties, scope |
| 5 | Leadership | Plan | Get leaders on board - top mgmt commitment, policy, roles |
| 6 | Planning | Plan | Make a plan - risk assessment, risk treatment, SoA, objectives |
| 7 | Support | Do | Get the support you need - resources, competence, awareness, docs |
| 8 | Operation | Do | Run it - executing the risk treatment plan day to day |
| 9 | Performance Evaluation | Check | Check how you did - monitoring, internal audit, mgmt review |
| 10 | Improvement | Act | Improve - nonconformity, corrective action, continual improvement |

## NIST CSF 2.0 — 22 Categories

| Function | Category Code | Category Name | Mnemonic |
|---|---|---|---|
| GOVERN | GV.OC | Organizational Context | "Our Risk Roles are Policed, Overseen, (via) Suppliers" --> |
| GOVERN | GV.RM | Risk Management Strategy | (2nd word: Risk) |
| GOVERN | GV.RR | Roles, Responsibilities, Authorities | (3rd word: Roles) |
| GOVERN | GV.PO | Policy | (4th word: Policed) |
| GOVERN | GV.OV | Oversight | (5th word: Overseen) |
| GOVERN | GV.SC | Cybersecurity Supply Chain Risk Mgmt | (6th word: Suppliers) |
| IDENTIFY | ID.AM | Asset Management | "Assets -> Risks -> Improve" (natural flow, 1st) |
| IDENTIFY | ID.RA | Risk Assessment | (2nd: Risks) |
| IDENTIFY | ID.IM | Improvement | (3rd: Improve) |
| PROTECT | PR.AA | Identity Mgmt, Authentication, Access Control | "Access, Awareness, Data, Platform, Infrastructure" (1st) |
| PROTECT | PR.AT | Awareness & Training | (2nd: Awareness) |
| PROTECT | PR.DS | Data Security | (3rd: Data) |
| PROTECT | PR.PS | Platform Security | (4th: Platform) |
| PROTECT | PR.IR | Technology Infrastructure Resilience | (5th: Infrastructure) |
| DETECT | DE.CM | Continuous Monitoring | "Cameras, Alarms" (1st: Cameras) |
| DETECT | DE.AE | Adverse Event Analysis | (2nd: Alarms) |
| RESPOND | RS.MA | Incident Management | "Manage -> Analyze -> Communicate -> Mitigate" (1st) |
| RESPOND | RS.AN | Incident Analysis | (2nd: Analyze) |
| RESPOND | RS.CO | Incident Response Reporting & Communication | (3rd: Communicate) |
| RESPOND | RS.MI | Incident Mitigation | (4th: Mitigate) |
| RECOVER | RC.RP | Incident Recovery Plan Execution | "Restore, then Report" (1st: Restore) |
| RECOVER | RC.CO | Incident Recovery Communication | (2nd: Report) |

## ISO/IEC 27001 Annex A — Commonly Cited Controls

| Control | Name | Used in this portfolio? | Memory Peg |
|---|---|---|---|
| A.5.1 | Policies for Information Security | Common reference | "5.1 = rule #1 of the org: have a policy" |
| A.5.15 | Access Control | Common reference | "5.15 = fifteen keys, only some doors open" |
| A.5.17 | Authentication Information | Used (Day 8 context) | "17, almost 18 - proving who you really are" |
| A.5.23 | Info Security for Cloud Services | Common reference | "5.23 = cloud in the sky" |
| A.8.2 | Privileged Access Rights | Common reference | "8.2 = two-tier access, admin vs user" |
| A.8.3 | Information Access Restriction | Used (Day 1) | "3 strikes and you're OUT" |
| A.8.5 | Secure Authentication | Used (Day 1) | "High-5 to log in" |
| A.8.7 | Malware Protection | Common reference | "Lucky 7, shield against malware" |
| A.8.8 | Management of Technical Vulnerabilities | Common reference | "8.8 looks like infinity - endless patch cycle" |
| A.8.9 | Configuration Management | Common reference | "8.9 = almost 10, baseline just before go-live" |
| A.8.10 | Information Deletion | Used (Day 8) | "Hit delete in 10 seconds" |
| A.8.12 | Data Leakage Prevention | Used | "Leak plugged at Gate 12" |
| A.8.16 | Monitoring Activities | Used (Day 7) | "Sweet 16 - someone's always watching" |
| A.8.17 | Clock Synchronization | Used | "17:00 in 24-hr time = 5 PM - literally a clock number" |
| A.8.20 | Networks Security | Used | "20/20 vision across the network" |
| A.8.23 | Web Filtering | Common reference | "8.23 = filter at the web gate" |
| A.8.24 | Use of Cryptography | Used (Day 8) | "24/7 encryption - always locked" |
| A.8.25 | Secure Development Life Cycle | Used (Day 6) | "25 stages/gates in the dev pipeline" |
| A.8.28 | Secure Coding | Used (Day 6) | "28 lines of clean code" |
