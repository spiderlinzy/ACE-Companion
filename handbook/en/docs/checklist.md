# Compliance Self-Check Checklist (Public Edition)

> This checklist compresses the book’s control points into checkable items for a first-round health check by an AI team. It is not legal advice and does not replace a conformity assessment for a specific system; run the “three-gap health check” first, then expand item by item across the governance foundation. Check states represent self-check conclusions only; formal compliance still requires applicable-law analysis and counsel input.

## I. Three-gap health check (answer these three groups first)

**Protection gap (before launch · at input)**

- [ ] System risk classification completed, with a documented rationale for whether it falls into a high-risk category
- [ ] Prohibited practices screened (manipulation, exploitation of vulnerabilities, improper scoring, etc.), with exclusion records retained
- [ ] Training / retrieval data has provenance and authorization records; representativeness and bias review performed
- [ ] Lawful basis and minimization measures in place for special-category (sensitive personal) data

**Oversight gap (during operation)**

- [ ] Key actions are logged, with recorded scope, retention period and access permissions
- [ ] Continuous monitoring and alert thresholds for output quality, drift and security metrics
- [ ] High-risk actions have human oversight and one-click stop / takeover capability
- [ ] Explicit risk-reassessment triggers: major functional change, scenario shift, major security incident, regulatory change, novel risk

**Remedy gap (after failure)**

- [ ] Incident grading, reporting deadlines, root-cause analysis and remediation closed-loop process defined
- [ ] User / affected-person notification and explanation scripts prepared
- [ ] Complaint channel, human review and correction channel available with a named owner

## II. Governance and documentation foundation

- [ ] AI system inventory maintained (see [Evidence Templates](evidence-templates.md)), covering in-house, purchased models and embedded components
- [ ] Risk register kept current along “pre-mitigation — post-mitigation — residual risk”
- [ ] Technical documentation maintained against Annex IV elements, with versions matched to system releases
- [ ] Provider / deployer status clarified; the three triggers for a deployer “becoming a provider” screened in contracts and design
- [ ] Vendors and model sources traceable; contracts define information provision, log cooperation and incident-notification duties
- [ ] Team completes role-appropriate AI literacy and security training, with training records retained

## III. Generative-AI specific controls

**Prompt injection and excessive authority**

- [ ] System instructions and external content architecturally separated; external content cannot rewrite high-trust rules by default (PTB)
- [ ] Tool / plugin calls use an allowlist, least privilege and mandatory human confirmation for dangerous actions
- [ ] Filtering and instruction-hierarchy constraints for indirect injection (retrieved documents, web pages, tool returns)

**Data and privacy**

- [ ] Sensitive-information detection and masking applied to retrieval corpus and context, preventing confidential / personal data from entering external models
- [ ] Data retention, deletion and “model not trained on inputs” contractual settings explicitly configured

**Hallucination and output reliability**

- [ ] Factual answers prioritize grounding in trusted sources; output confidence constrained by source tier (FTH)
- [ ] High-risk conclusions carry citations and uncertainty notes; explicit refusal or human handoff when no source exists
- [ ] Output layer validates unsafe content and out-of-scope formats, rather than relying only on input filtering

**Verification and launch**

- [ ] Benchmark and red-team testing completed before launch; test sets, attack cases and results retained
- [ ] Acceptance thresholds set as illustrative rather than “industry universal,” calibrated to the organization’s own false-accept / false-reject costs
- [ ] Post-launch evaluation-set regression mechanism established; core security cases rerun after model upgrades

## IV. Suggested implementation order by priority

1. **P0 (stay alive)**: asset inventory, risk register, log traceability, human takeover, data masking, layered prompt-injection defense.
2. **P1 (auditable)**: technical documentation, vendor contract clauses, output validation and citation grounding, monitoring alerts, incident-response plan.
3. **P2 (systematic)**: maturity model, compliance governance platform, automated evidence collection, standing red teaming, training and drills.

← [Evidence Artifact Templates](evidence-templates.md) ｜ Next: [Verification & Red Teaming](verification.md)
