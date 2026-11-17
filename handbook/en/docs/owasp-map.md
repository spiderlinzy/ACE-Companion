# OWASP LLM Top 10 Crosswalk

The OWASP Top 10 for LLM Applications is the de-facto industry risk list for generative-AI systems. It **is not a regulation and carries no penalties**, but it provides a quick index from attack categories to Act obligations and engineering countermeasures. The mapping is approximate: one attack category usually triggers several articles, and one article covers several attack categories. Treat this table as an entry index, not as legal interpretation.

| OWASP LLM | Attack category | Most directly triggered Act obligations | Book countermeasures |
|---|---|---|---|
| LLM01 | Prompt Injection | Art. 15(5) robustness against adversarial manipulation; Art. 14 human oversight | Prompt-injection defense; tool-call controls |
| LLM02 | Insecure Output Handling | Art. 15(1) accuracy; Art. 15(4) robustness; Art. 72 post-market monitoring | Output validation layer; “validate output first” design |
| LLM03 | Training Data Poisoning | Art. 10 data governance; Art. 15(5) cybersecurity | Data compliance foundation; RAG data hygiene |
| LLM04 | Model Denial of Service | Art. 15(1) performance under declared conditions; Art. 15(4) robustness | Benchmarking (capacity ceiling as a test case) |
| LLM05 | Supply-Chain Vulnerabilities | Art. 25(1) provider-inheritance trigger; Art. 53 GPAI downstream information; Art. 13 information to deployers | Supply-chain security; Art. 25 trigger screening |
| LLM06 | Sensitive Information Disclosure | Art. 10(5) special-category data; GDPR overlap; Art. 50 transparency touchpoints | Data compliance; PII leakage incident case |
| LLM07 | Insecure Plugin Design | Art. 15(5) cybersecurity; Art. 14 oversight design | Tool-call allowlist and plugin governance |
| LLM08 | Excessive Agency | Art. 14(1)(3)(4) human oversight; Art. 26(2) deployer oversight assignment | Least privilege and mandatory human confirmation |
| LLM09 | Overreliance | Art. 14 human oversight; Art. 4 AI literacy; Art. 86 right to explanation | PTB/FTH trust boundaries; governance training |
| LLM10 | Model Theft | Art. 15(5) cybersecurity; trade-secret protection under national law | Red teaming (attacker-perspective probing); access control |

## Two reading notes

**First, no article in the Act is called “prompt injection.”** The Act reaches this harm through robustness (Art. 15(5)) and oversight (Art. 14) — which is exactly why “compliance translation” exists: translate attack language into regulatory language, then back into control design.

**Second, the three thinnest engineering coverages — LLM04 denial of service, LLM07 plugin design and LLM10 model theft — correspond precisely to the three most generally worded rows of the Act.** When advancing compliance under the proportionality principle, these risks follow the same evidence discipline as the rest, but the artifact templates can be lighter; effort need not be spread evenly.

← [Regulation–Evidence Map](regulation-map.md) ｜ Next: [Evidence Artifact Templates](evidence-templates.md)
