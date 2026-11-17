<div class="hero">
  <h1>AI Compliance Engineering</h1>
  <div class="sub">From Regulation to Evidence: A Methodology for Trustworthy and Ethical AI Systems<br/>Translating regulatory and policy obligations into deployable technical controls, and proving control effectiveness with auditable evidence.</div>
  <div class="badges"><span>Author: ZhiXuan ZHU</span><span>AI Compliance · LLM Security · Risk Governance</span><span>ISBN 979-8-16714-909-0</span></div>
</div>

## What this site covers

Regulatory requirements are written in legal and policy language, while AI systems are built from code, architectures and operating processes. Governance frameworks (such as NIST AI RMF, ISO/IEC 42001 and the EU Artificial Intelligence Act) state *what should be done*, but rarely explain *how to implement it technically*; security engineering practices solve *how to control a specific risk*, but lack a systematic connection to regulatory requirements and evidence standards.

This site treats **Regulation — Controls — Evidence** as a single engineering problem, and consolidates a reusable translation method, mapping tables, self-check checklists and evidence templates. It is the public methodology companion to the book *AI Compliance Engineering*, shared for discussion, job applications and research presentation; the complete argumentation, cases and operational details follow the formal publication.

## Four method components

<div class="cards">
  <div class="card"><h4>CTF Compliance Translation Framework</h4><p>A framework that systematically translates abstract regulatory requirements into concrete technical controls and verification evidence through four abstraction levels.</p></div>
  <div class="card"><h4>RCE Risk–Control–Evidence Loop</h4><p>Risk-Control-Evidence: risk identification, control implementation and evidence generation form a closed iterative loop rather than disconnected activities; the evidence to be produced is specified at the control design stage.</p></div>
  <div class="card"><h4>PTB Prompt Trust Boundary</h4><p>Models the permission boundary between system instructions, developer configuration and untrusted external content in generative AI. The core rule: low-trust information must not modify high-trust rules.</p></div>
  <div class="card"><h4>FTH Fact Trust Hierarchy</h4><p>The confidence of a generated claim must not exceed the trust level of the sources it relies on; a source constraint for retrieval-augmented and tool-output generation.</p></div>
</div>

> Scope note: CTF and RCE are organizational frameworks used to integrate established practices; PTB and FTH are design propositions (conceptual models) that have not yet been formally validated as predictive models and should not be used as quantitative laws.

## Contents

- [Methodology Framework](docs/framework.md): definitions, relationships and applicability boundaries of the four components.
- [Regulation–Evidence Map](docs/regulation-map.md): core obligations of the EU Artificial Intelligence Act → required evidence artifacts → corresponding engineering methods.
- [OWASP LLM Top 10 Crosswalk](docs/owasp-map.md): jump from attack categories to Act obligations and countermeasure chapters.
- [Evidence Artifact Templates](docs/evidence-templates.md): ready-to-use tables for the AI system inventory, risk register and Annex IV technical documentation list.
- [Compliance Self-Check Checklist](docs/checklist.md): the “three gap” health check and governance checklist for before input, during operation and after failure.
- [Verification & Red Teaming](docs/verification.md): verification approaches for benchmarking, red teaming, explainability and continuous monitoring.
- [Chapter Guide](docs/chapters.md): structural map of the book’s 16 chapters and appendices.
- [Glossary](docs/glossary.md): quick reference for CTF / RCE / PTB / FTH, RAG, prompt injection, FRIA, GPAI and other terms.
- [About & Disclaimer](docs/about.md)

<div class="book-cta">
  <strong>Published book: <em>AI Compliance Engineering: From Regulation to Evidence — A Methodology for Trustworthy and Ethical AI Systems</em></strong><br/>
  Full chapters, an end-to-end case study and Appendices A–D (methodology and regulation–evidence index) are available in the paperback and eBook.
  <br/><a class="btn" href="https://www.amazon.com/dp/B0HQDC7HJ2" target="_blank" rel="noopener">View the book on Amazon</a>
</div>

## Who this is for

- **AI / security engineers** who need to write compliance requirements into architectures and code;
- **Compliance and risk staff** responsible for AI risk, internal control, audit and due diligence;
- **Technical managers and product owners** evaluating high-risk AI deployment;
- **Researchers and students** following AI governance, algorithmic fairness and generative-AI security.

---

*The content on this site is methodology education and engineering reference; it does not constitute legal advice. For a specific compliance decision, consult qualified counsel for the relevant jurisdiction, sector and use case.*
