# Verification & Red Teaming

> A control “designed” is not a control “effective.” Verification answers: **is there reproducible evidence that the control holds under real attacks and real workloads?** This page is a guide to verification methods; full operating steps, case design and metric definitions appear in Chapters 9–12 and Appendix A of *AI Compliance Engineering*.

## Four complementary verification methods

| Method | Question it answers | Typical evidence | Main chapter |
|---|---|---|---|
| **Benchmark** | Whether accuracy, latency and capacity meet targets on standard datasets and workloads | Test-set version, metric results, P95 latency, capacity ceiling | Ch. 9 |
| **Red Teaming** | Whether a motivated attacker can bypass controls, induce unauthorized actions or exfiltrate information | Attack-case library, success rate, reproduction steps, fix-regression record | Ch. 10 |
| **Explainability & Fairness Assessment** | Whether decision reasons can be explained, and whether performance differs significantly across groups | Feature / attribution notes, group metrics, bias-review record | Ch. 11 |
| **Continuous Monitoring & Incident Drills** | Whether post-launch performance drift and security incidents are detected and handled in time | Monitoring dashboard, alert records, incident timeline and post-mortem report | Ch. 12 |

## Shared discipline of verification design

- **Fix the test set and versions**: archive model version, prompt version, knowledge-base snapshot and test-case version together so results are reproducible and comparable.
- **Define metrics before measuring**: for attack success rate (ASR), hallucination rate, citation accuracy or false-accept / false-reject rates, specify numerator, denominator and decision rule up front instead of picking numbers after the fact.
- **Thresholds are illustrative references, not industry-wide standards**: the specific percentage thresholds in the book demonstrate the method; organizations should calibrate them to their own risk appetite, user impact and error costs rather than copy them outright.
- **Report confidence intervals and sample sizes**: ratios from small samples (e.g. 100–250 cases per category) carry statistical fluctuation; report intervals rather than single point values.
- **Close the loop on red-team findings**: every exploitable issue maps to a control fix, a regression case and a review date, avoiding “archive immediately after testing.”

## The basic red-team loop

1. **Define objective and boundaries**: target under test, authorization scope, permitted attack techniques, prohibited destructive actions.
2. **Model threats**: list attack hypotheses starting from the OWASP LLM Top 10 and real business-abuse paths.
3. **Execute probing**: cover prompt injection, unauthorized tool calls, sensitive-information elicitation, unsafe output and excessive agency.
4. **Rate and reproduce**: grade by exploitability and business impact; retain minimal reproduction prompts and conversation traces.
5. **Fix and regress**: layered defense (input — model — output — permission — audit); rerun the same case set after fixing.
6. **Convert into monitoring rules**: turn one-off attack cases into standing post-launch detection signals.

## Link to compliance evidence

Verification reports are not internal technical material; they directly support key artifacts in the regulation–evidence map: Art. 15 robustness and cybersecurity evidence, Art. 9 risk-management iteration records, Art. 72 post-market monitoring and Art. 73 incident handling. **Without verification evidence, control claims remain assertions rather than proof in an audit or enforcement proceeding.**

← [Compliance Self-Check Checklist](checklist.md) ｜ Next: [Chapter Guide](chapters.md)
