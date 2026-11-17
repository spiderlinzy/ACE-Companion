# Evidence Artifact Templates

> Regulators usually ask three questions first: “What AI systems do you have?”, “How are the risks managed?”, and “Where is the technical documentation?” The three templates below answer those questions. They can be copied directly into Excel, LibreOffice Calc or Google Sheets; array formulas are deliberately avoided so recalculation stays consistent across spreadsheet software. These are methodology examples; field details must be adapted to the applicable jurisdiction and use case.

## Template 1: AI System Inventory & Classification Register (Art. 3(1), Annex III)

The final risk-tier column is an engineering classification (L0–L3, by control strength), not the Act’s legal classification; the Act’s own categories are Annex I / Annex III / non-high-risk.

| # | System name | Deploying party | Vendor / model source | Purpose and scope | Is it an “AI system”? | Annex III area (if any) | Annex I product (if any) | Risk tier L0–L3 | FRIA required? | Evidence owner |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Résumé screening tool | HR | Vendor X, model Y | Hiring screening | Yes | Annex III point 4, employment | — | L1 High | Required for public bodies |  |
| 2 |  |  |  |  |  |  |  |  |  |  |
| 3 |  |  |  |  |  |  |  |  |  |  |

## Template 2: High-Risk AI Risk Register (Art. 9)

The risk management system is a continuously iterated process, not a one-off document. Score severity × likelihood (5×5) once before mitigation and once after; **the residual-risk column is what persuades regulators**.

| # | Risk scenario | Source (intended purpose / reasonably foreseeable misuse / lifecycle) | Severity 1–5 | Likelihood 1–5 | Pre-mitigation score | Mitigation controls (chapter) | Post-mitigation score | Residual risk and rationale | Review date |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Prompt injection induces the assistant to perform a harmful action | Reasonably foreseeable misuse | 5 | 4 | 20 | Layered defense; mandatory human interception | 2 | Under the tested attacks, residual attack success rate (ASR) lies within the accepted band; accepted with rationale |  |
| 2 |  |  |  |  |  |  |  |  |  |
| 3 |  |  |  |  |  |  |  |  |  |

## Template 3: Annex IV Technical Documentation Element Checklist (Art. 11)

Technical documentation should be compiled before market placement and kept current; mapping every element to an owner and status turns it into an accountable, living artifact rather than a pile of drafts.

| Annex IV element | What must be established | Evidence owner | Status (draft / complete / reviewed) | Review date |
|---|---|---|---|---|
| (1) General description of the system, intended purpose and provider | Scope, objective, what the system does | Product owner |  |  |
| (2) System components and development-process description | Architecture, models, data and development methods | Technical lead |  |  |
| (3) Data governance and training / validation / test data | Provenance, relevance, bias examination (Art. 10) | Data lead |  |  |
| (4) Risk management system | Risks, mitigation, residual risk (Art. 9) | Risk lead |  |  |
| (5) System monitoring, operation and control means | Logs, human oversight, intervention capability (Art. 12, 14) | Operations lead |  |  |
| (6) Accuracy, robustness and cybersecurity | Metrics, testing, adversarial robustness (Art. 15) | Security lead |  |  |
| (7) Changes made by the provider | Version history, substantial-modification triggers (Art. 25) | Change manager |  |  |
| (8)–(14) Remaining elements | Conformity assessment, pre-established changes, instructions for use, etc. | Compliance lead |  |  |

## Usage discipline

- Every piece of evidence **has a date, a version and an owner**, so it cannot be back-filled without proving when it was formed;
- Evidence must be independently reproducible: archive the test-set version, model version, prompt version and scoring rules together;
- The register exists not to “fill a table” but to reconstruct, during an incident investigation or conformity assessment, “what information was available and what decision was made at the time.”

← [OWASP Crosswalk](owasp-map.md) ｜ Next: [Compliance Self-Check Checklist](checklist.md)
