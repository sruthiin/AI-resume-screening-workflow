# Requirements

## Functional Requirements
| ID | Requirement | Verification Method |
|---|---|---|
| FR-001 | Accept synthetic job description | Input test |
| FR-002 | Accept synthetic resume | Input test |
| FR-003 | Extract relevant resume skills | Extraction tests |
| FR-004 | Extract relevant experience evidence | Extraction/evidence tests |
| FR-005 | Extract job requirements | Requirement extraction tests |
| FR-006 | Compare evidence with requirements | Matching tests |
| FR-007 | Identify potential gaps | Gap/unknown tests |
| FR-008 | Produce structured candidate summary | Output schema tests |

## AI Quality Requirements
| ID | Requirement | Verification Method |
|---|---|---|
| AIR-001 | Use only supplied information | Hallucination tests |
| AIR-002 | Do not invent skills, employers, durations, certifications, achievements or metrics | Hallucination tests |
| AIR-003 | Separate evidence from assumptions | Grounding review |
| AIR-004 | Mark missing information rather than guessing | Gap/ambiguity tests |
| AIR-005 | Provide evidence for important claims | Evidence-mapping tests |
| AIR-006 | Avoid irrelevant personal attributes in suitability analysis | Paired fairness tests |

## Responsible-AI Controls
1. Final decision remains human-owned.
2. Irrelevant demographic/personal information must not drive job matching.
3. AI claims must be reviewable against source text.
4. Synthetic data must be used in the portfolio.
5. Unknowns and uncertainty must be visible.
