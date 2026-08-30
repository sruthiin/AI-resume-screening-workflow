# Findings

> This file must be completed only after actual model executions and evaluation. Do not pre-fill outcomes.

## Executive Finding
**Status:** Pending actual LLM execution.

## V1 Observations
Record observed baseline behavior only.

- What was extracted correctly?
- What was missing or over-inferred?
- What evidence was not traceable?
- Did the output distinguish uncertainty?

## V2 Observations
Record actual changes relative to comparable V1 tests.

- Did evidence grounding improve?
- Did hallucination behavior change?
- Did irrelevant personal information remain excluded?
- Were there any new trade-offs or formatting problems?

## V3 Observations
Record actual changes relative to comparable V2 tests.

- Did structure improve reviewer usability?
- Were Unknowns and risks visible?
- Did the model respect the human decision boundary?
- Did structured output introduce any failure modes?

## Hallucination Findings
Record only observed failures or successful controls, linked to Test IDs.

## Fairness Findings
Compare RES-005A and RES-005B using the same prompt and JD. Describe only observed differences and whether they affect job-related assessment.

## Defect Findings
Summarize meaningful defects from `defect-log.xlsx`.

## Risk Findings
Summarize residual risks after applying prompt and workflow controls.

## Trade-offs
Document cases where a stronger guardrail reduced over-inference but also reduced semantic matching, or where structured output improved reviewability but increased verbosity.

## Limitations
- Synthetic data is not representative of all real-world resumes.
- LLM behavior can vary by model, system configuration, and generation settings.
- Portfolio tests do not establish production accuracy or legal compliance.
- A small test set cannot prove absence of bias or hallucination.
