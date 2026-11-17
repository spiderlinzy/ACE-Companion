# Methodology Framework

## The core problem

A specific gap exists at the intersection of AI regulation and engineering practice: **regulatory requirements are expressed in legal and policy language, while AI systems are built from code, architectures and operating processes; there is no widely adopted end-to-end methodology for translating the former into the latter and proving with verifiable evidence that the translation works.**

Each of the three existing families of methods remains incomplete:

- **Governance frameworks** (NIST AI RMF, ISO/IEC 42001, the EU AI Act) define *what should be done* but do not explain *how* to implement it technically.
- **Security engineering practices** (prompt-injection defense, content moderation, red teaming) solve *how* to control specific risks but lack a systematic connection to regulatory requirements and evidence standards.
- **AI Assurance literature** focuses on *evidence*, but mostly treats evidence as a post-hoc evaluation activity rather than an integrated component of system design and operation.

This framework argues for treating **regulation, controls and evidence** as a single engineering problem.

## Four method components

| Component | Problem it solves | Nature |
|---|---|---|
| **CTF Compliance Translation Framework** | How to systematically translate abstract regulatory requirements into concrete technical controls and verification evidence | Organizational framework: a four-layer, three-function translation structure |
| **RCE Risk–Control–Evidence Loop** | How risk identification, control implementation and evidence generation form a closed iterative loop instead of disconnected activities | Architectural pattern: extends the PDCA cycle with AI-specific evidence types and risk-reassessment triggers |
| **PTB Prompt Trust Boundary** | How to model and enforce the permission boundary between system instructions, developer configuration and untrusted external content | Design proposition: five trust levels and violation rules; not yet empirically validated as a predictive model |
| **FTH Fact Trust Hierarchy** | How to reason about the confidence of generated outputs from the trustworthiness of their sources | Design proposition: output confidence is constrained by source trust level; consistent with RAG grounding practice |

## Where it adds value

- **Relative to NIST AI RMF / ISO/IEC 42001**: the latter two are organizational management systems; this framework fills the **technical implementation layer** — how a single regulatory article travels through the abstraction layers to code and evidence. The two are complementary, not competing.
- **Relative to prompt-injection defense**: input filtering, output validation, system-prompt isolation and sandboxing can be understood as enforcing one shared principle — **low-trust information must not modify high-trust rules**. PTB does not invent new defensive techniques; it provides a vocabulary for reasoning about why a defense works and where it fails.
- **Relative to hallucination mitigation**: RAG grounding, fact-checking and confidence scoring are standard practices; FTH extends the rule “claim confidence must not exceed source trust level” from retrieval settings to model parametric knowledge, tool outputs and user input.
- **Relative to AI Assurance**: RCE moves evidence generation forward into the **control design stage** — every control specifies at design time what evidence it produces and how that evidence is verified, turning assurance from an audit action into an engineering requirement.

## Applicability boundaries

**It can support:**

- A structured methodology for translating regulatory requirements into technical controls;
- A shared vocabulary and reference architecture for internal discussion of AI Compliance Engineering (ACE);
- Checklists, metrics and failure boundaries for common risk categories (prompt injection, hallucination, data privacy, agent security);
- A phased compliance capability-building roadmap;
- A documentation basis for internal control audits and due diligence.

**It cannot support:**

- **Quantitative predictive power for PTB/FTH**: the five levels have not been empirically tested against real attack success rates or hallucination frequency; they are design heuristics, not prediction tools;
- **Legal compliance assurance**: this is an engineering methodology, not legal advice; compliance determinations require qualified legal counsel;
- **Security guarantees against unknown attacks**: zero-days, novel jailbreaks and emergent behavior may bypass existing controls;
- **Performance benchmarks for specific commercial products**: no specific platform, security product or model vendor is evaluated;
- **Adjudication of ethical value trade-offs**: the framework identifies ethical tensions (efficiency vs. fairness, autonomy vs. automation); value choices require organizational and societal deliberation.

> The terms CTF / RCE / PTB / FTH are naming conventions for a shared vocabulary within the framework; the underlying ideas overlap with established concepts in requirements engineering, systems theory and AI safety. The contribution lies in their specific combination and their application to AI compliance engineering.

← [Home](../README.md) ｜ Next: [Regulation–Evidence Map](regulation-map.md)
