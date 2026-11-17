# Regulation–Evidence Map

> This page is a public selected edition of the book’s master skeleton index. It maps the core obligations of the EU Artificial Intelligence Act (Regulation (EU) 2024/1689, calibrated against the 2026 Digital Omnibus, Regulation (EU) 2026/1744) to **auditable evidence artifacts** and the **engineering methods that produce them**. This page cannot replace the legal text; the official text and the enforcement guidance of competent authorities govern exact wording and scope.

## The three-step chain: Obligation → Evidence artifact → Method

- **Obligation**: what the Act requires an actor (provider, deployer, general-purpose AI model provider, importer or distributor) to do.
- **Evidence artifact**: specific, auditable and reproducible material proving that an obligation has been fulfilled — the “Evidence” half of the RCE loop.
- **Corresponding method**: the engineering methods and frameworks that produce the artifact (CTF / RCE / PTB / FTH).

Coverage: **● Strong coverage** (a dedicated method chapter exists) ｜ **◐ Partial coverage** (touched on, but templates or anchors still needed) ｜ **○ Gap** (artifact identified, content to be added later).

## Three-gap health check (run this first)

Before reading the full map, run a “three-gap health check” along the system lifecycle:

- **Protection gap (at input)**: before data enters the system, can it resist bias and data misuse? Corresponds to the prohibited practices in Article 5, data governance in Article 10 and the Fundamental Rights Impact Assessment (FRIA) in Article 27.
- **Oversight gap (during operation)**: does the system run visibly and auditably? Corresponds to logging in Article 12, the quality management system in Article 17 and post-market monitoring in Article 72.
- **Remedy gap (after failure)**: can affected persons understand, challenge and correct decisions? Corresponds to serious-incident reporting in Article 73, the right to complaint in Article 85, the right to explanation in Article 86 and information to affected persons under Article 26(11).

## Horizontal obligations (apply to all AI systems)

| Article & obligation | Required evidence artifact | Corresponding method | Coverage |
|---|---|---|---|
| **Art. 4** AI literacy (all actors; converted from an obligation of result to an obligation of means) | Training register: content, audience, date | Governance platform; implementation roadmap | ◐ |
| **Art. 5** Prohibited practices (8 categories applicable from 2025-02-02; bans on CSAM generation and non-consensual intimate imagery apply from 2026-12-02) | Prohibition screening record and design-exclusion evidence | Four-tier risk grading; roadmap | ○ |
| **Art. 50** Transparency obligations (chatbot disclosure, machine-readable marking, emotion-recognition notice, deepfake / public-interest text labeling; applies from 2026-08-02; existing-machine marking completed by 2026-12-02) | Transparency touchpoint register, disclosure wording, machine-readable marking template | Generative-AI controls; roadmap | ◐ |

## High-risk AI system obligations (Annex III: 2027-12-02; Annex I: 2028-08-02)

| Article & obligation | Required evidence artifact | Corresponding method | Coverage |
|---|---|---|---|
| **Art. 6 + Annex I/III** Risk classification and exit filters | Per-system classification record, with a reasoned decision when an exit filter is invoked | Four-tier risk grading | ● |
| **Art. 9** Risk management system | Risk register: 5×5 scoring, mitigation tracking, residual-risk statement, iteration log | RCE loop; continuous monitoring; end-to-end case | ● |
| **Art. 10** Data and data governance | Data governance checklist: provenance, representativeness, error / bias examination, special-category data permission | Data compliance foundation | ● |
| **Art. 11 + Annex IV** Technical documentation | Technical documentation compiled against the 14 elements of Annex IV, with owner and status marked item by item | CTF framework | ◐ |
| **Art. 12** Record-keeping and logs (deployer retention under Art. 26(6)) | Log configuration record: scope recorded, retention period (at least 6 months for deployers), access control | Continuous monitoring & incident response | ● |
| **Art. 13** Transparency information to deployers | Deployer information pack: capabilities, limitations, intended purpose, declared performance | Supply-chain security; CTF | ◐ |
| **Art. 14** Human oversight (provider design obligation; deployer assignment obligation under Art. 26(2)) | Oversight design document: human–machine interface, override capability, training record, automation-bias assessment | PTB/FTH trust boundaries; agent permission control | ◐ |
| **Art. 15** Accuracy, robustness and cybersecurity | Benchmark report, red-team report, adversarial and robustness test evidence, security assessment | Core security controls; benchmarking; red teaming | ● |
| **Art. 17** Quality management system (QMS) | QMS documentation: procedures, version control, nonconformity handling | Governance platform & maturity model | ◐ |
| **Art. 43** Conformity assessment (internal control / notified body routes) | Assessment record, route-selection rationale, description of alternatives | Roadmap (position of assessment in the timeline) | ○ |
| **Art. 47–49** EU declaration of conformity, CE marking, registration | Declaration of conformity, CE affixing record, EU database registration entry | Roadmap | ○ |
| **Art. 71** EU database registration | Database entry: key system identifiers and document links | Roadmap | ○ |

## Deployer obligations

| Article & obligation | Required evidence artifact | Corresponding method | Coverage |
|---|---|---|---|
| **Art. 25** When a deployer becomes a provider (three triggers: affixing its own trademark, substantial modification, change to a high-risk use) | Procurement-trigger screening, supply-chain due-diligence record, contractual information rights | Supply-chain security | ◐ |
| **Art. 26** Deployer obligations (12 paragraphs covering oversight assignment, log retention, monitoring, incident notification, information to affected persons, cooperation, etc.) | Deployer evidence file: assignment records, log retention, instructions for use, incident-notification log, notification templates | Monitoring & incident response; roadmap | ◐ |
| **Art. 27** Fundamental Rights Impact Assessment (public-sector deployers of Annex III point 4 systems) | FRIA report: use scenario, fundamental-rights risks, mitigation measures | Dedicated artifact to be added | ○ |

## General-Purpose AI Model (GPAI) obligations (Chapter V, applicable from 2025-08-02)

| Article & obligation | Required evidence artifact | Corresponding method | Coverage |
|---|---|---|---|
| **Art. 51–52** Systemic-risk GPAI models (10²⁵ FLOP presumption and rebuttal; two-week notification duty) | Systemic-risk assessment: training-compute evidence, rebuttal record, copy of notification | To be added | ○ |
| **Art. 53** GPAI provider obligations (Annex XI technical documentation, Annex XII downstream information, copyright policy, training-content summary) | Model documentation, downstream information sheet, copyright policy, training-content summary | Downstream supply-chain handoff (partial) | ○ |
| **Art. 54–56** Third-country authorized representative, limits of the open-source exemption, code of practice | Open-source exemption compliance statement, code-of-practice adherence record, standards-gap document | To be added | ○ |

## Post-market, remedies and enforcement

| Article & obligation | Required evidence artifact | Corresponding method | Coverage |
|---|---|---|---|
| **Art. 72** Post-market monitoring | Monitoring plan and report: drift detection, performance tracking, reassessment triggers | Continuous monitoring; end-to-end case | ● |
| **Art. 73** Serious-incident reporting (competent authority within 15 days; 24 hours for serious public-safety risk) | Incident report: grading, timeline, root-cause analysis, evidence that the system was not altered | Incident response; case file | ◐ |
| **Art. 85–87** Right to complaint, right to explanation, whistleblower protection | Complaint-handling record, explanation mechanism and decision-logic mapping | Explainability & fairness (partial) | ○ |
| **Art. 99–101** Penalties (three tiers: €35 million / 7% of global turnover; €15 million / 3%; €7.5 million / 1%; GPAI systemic-risk tier €30 million / 6%) | Penalties are not an artifact — a complete, dated and verifiable evidence file is the defensive posture in enforcement | Roadmap (budget & sequencing); governance | ○ |

## Model vs system: who owes what

The Act regulates **models** and **systems** in different chapters, timelines and enforcers; this is the main source of confusion in the GPAI chapter:

| Obligation holder | Where the obligation sits | Typical actor | Enforcer | Example obligations |
|---|---|---|---|---|
| GPAI **model** (Chapter V) | Art. 53; Art. 51–52, 55 | Model provider (including a fine-tuner that constitutes a substantial modification) | Commission through the AI Office (Art. 101) | Annex XI technical documentation, Annex XII downstream information, copyright and training summary |
| AI **system** (Chapters II–III) | Art. 5, 9–15, 17, 43, 50 | System provider / deployer | National market-surveillance authorities (Art. 99) | Risk management, data governance, technical documentation, CE marking, registration |
| System **deployer** | Art. 26–27 | Deployer | National authorities | Human oversight, logs, FRIA, information to affected persons |

> A deployer becomes a provider by affixing its name, making a substantial modification or changing to a high-risk use (Art. 25); a fine-tuner becomes a GPAI model provider only when the modification is judged substantial under Art. 3(63) and Chapter V — a legal judgment that cannot be inferred directly from a particular fine-tuning technique. Both transitions should be screened at design time, because the evidence obligations flip immediately.

← [Methodology Framework](framework.md) ｜ Next: [OWASP LLM Crosswalk](owasp-map.md)
