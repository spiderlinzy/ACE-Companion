# Glossary

> A web quick-reference of the book’s core terms; usage here follows the book’s definitions. For standard definitions, consult the corresponding regulations and official documents.

**AI Compliance Engineering (ACE)**
The engineering discipline and practice of translating regulatory requirements into technical controls and proving control effectiveness with verifiable evidence.

**CTF Compliance Translation Framework**
An organizational framework that translates abstract regulatory requirements through several abstraction layers into concrete controls and verification evidence.

**RCE Risk–Control–Evidence Loop**
An architectural pattern in which risk identification, control implementation and evidence generation are linked and continuously iterated; every control specifies its evidence at the design stage.

**PTB Prompt Trust Boundary**
A model distinguishing the trust levels of system instructions, developer configuration and untrusted external content; the core rule is that low-trust information must not modify high-trust rules.

**FTH Fact Trust Hierarchy**
A model constraining generated-content confidence by source trustworthiness: a claim’s confidence must not exceed the trust level of the sources on which it relies.

**RAG Retrieval-Augmented Generation**
An architecture that retrieves relevant material from an external knowledge base before generating an answer, grounding model output in the retrieved results.

**Prompt Injection**
An attack in which an attacker alters model instructions or bypasses constraints through user input or external content (web pages, documents, tool returns); indirect injection arrives via retrieved external content.

**Hallucination**
Model-generated content that looks plausible but lacks factual basis or contradicts the sources.

**ASR Attack Success Rate**
In red teaming, the proportion of attack cases that achieve the intended violation effect; one measure of defensive effectiveness; interpreted only with a fixed case set and sample size.

**FRIA Fundamental Rights Impact Assessment**
An assessment required by the EU AI Act for certain public-sector deployers of high-risk systems, examining the impact on fundamental rights.

**QMS Quality Management System**
A procedural management system organizations establish to assure process and product quality; Art. 17 of the Act requires it of providers.

**GPAI General-Purpose AI Model**
A foundation model with significant generality that can be integrated into many downstream systems; Chapter V of the Act sets separate obligations for its providers.

**High-Risk AI System**
A risk category under the Act classified by use and risk; Annex III lists employment, credit, critical infrastructure, law enforcement, migration and other areas, while Annex I covers systems serving as product safety components; high-risk systems carry the most complete set of obligations.

**Conformity Assessment**
The process by which a provider demonstrates that a high-risk system meets the Act’s requirements, via internal control (Annex VI) or a notified body (Annex VII).

**Post-Market Monitoring**
Activities after a system is placed on the market to continuously collect performance and incident data, detect drift and trigger correction (Art. 72).

**OWASP LLM Top 10**
The OWASP top-ten security-risk list for LLM applications; an industry factual reference, not a regulation.

**Red Teaming**
Security testing in which an independent perspective actively simulates attackers, probes system weaknesses and produces reproducible findings.

**Least Privilege**
Agents, tools and accounts are granted only the minimum access scope and action permissions required to complete the task.

← [Chapter Guide](chapters.md) ｜ Next: [About](about.md)
