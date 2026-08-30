# Risk & Control Matrix

| Risk | Impact | Control | Evidence to Monitor |
|---|---|---|---|
| Hallucinated qualification | High | Evidence grounding + human review | Unsupported claims in outputs |
| Bias from irrelevant attributes | Critical/High | Ignore irrelevant attributes + paired tests | Difference between paired outputs |
| False positive match | High | Require explicit evidence | Match without source evidence |
| False negative match | High | Human review of terminology/context | Legitimate evidence missed |
| Privacy exposure | High | Synthetic data + minimum necessary fields | Unnecessary personal information surfaced |
| Autonomous decision | Critical | Explicit prohibition + human checkpoint | Accept/reject language or recommendation |
| Overconfidence | High | Show Unknown and uncertainty | Missing evidence presented as certainty |

## Control Ownership
The fictional workflow assumes the recruiter/human reviewer owns the final decision. AI output is advisory evidence organization only.
