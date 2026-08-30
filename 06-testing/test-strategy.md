# Test Strategy

## Purpose
Validate whether the AI-assisted workflow extracts requirements and candidate evidence accurately, maps evidence to requirements without unsupported inference, surfaces uncertainty, resists hallucination, ignores irrelevant personal attributes, and preserves human decision authority.

## Test Principles
- Use the same JD/resume combinations for comparable tests.
- Record the actual model output exactly enough for independent review.
- Evaluate against predefined expectations before reviewing the output for defects.
- Log meaningful defects, including severity and evidence.
- Retest comparable scenarios after prompt changes.
- Never fabricate pass/fail results, scores, improvement percentages or findings.

## Suggested Test Set
22 tests covering:
- Normal matching: 4
- Partial/gaps: 4
- Terminology: 3
- Missing/vague evidence: 3
- Hallucination: 3
- Bias/fairness: 3
- Decision boundary: 2

A consistency comparison can be performed across selected paired tests and recorded in notes.

## Execution Protocol
For each test:
1. Copy the selected JD and resume into the selected prompt version.
2. Record model/tool and execution date.
3. Save the output in a local evidence file or screenshot.
4. Compare the output against Expected Behavior.
5. Mark Pass / Fail / Needs Review.
6. Record defect details where applicable.
7. Do not edit the model output before saving evidence.

## Test Categories
### Normal Matching
Checks direct evidence extraction and evidence-backed matching.

### Partial / Gaps
Checks that missing requirements are surfaced without invented evidence.

### Terminology
Checks useful semantic equivalence without over-inference.

### Missing / Vague Evidence
Checks the Unknown state and prevents specific tool inference.

### Hallucination
Checks invented qualifications, duration, certifications, responsibilities or metrics.

### Bias / Fairness
Uses RES-005A and RES-005B with identical job-related qualifications but different irrelevant personal details.

### Decision Boundary
Tests requests that explicitly ask the AI to decide whether to hire/reject.
