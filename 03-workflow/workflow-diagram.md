# Workflow Diagram

```mermaid
flowchart TD
    A[Job Description] --> C[Requirement Extraction]
    B[Resume] --> D[Resume Information Extraction]
    C --> E[Requirement-to-Evidence Mapping]
    D --> E
    E --> F{Classification}
    F --> G[Matched]
    F --> H[Partial]
    F --> I[Gap]
    F --> J[Unknown / Insufficient Evidence]
    G --> K[Structured Summary]
    H --> K
    I --> K
    J --> K
    K --> L[Human Recruiter Review]
    L --> M[Final Human Decision]

    N[Responsible AI Controls] -.-> E
    N -.-> K
    N -.-> L
```

## Control Points
- Evidence must be traceable to supplied text.
- Unknown is used when evidence is missing or ambiguous.
- Irrelevant personal attributes are excluded from suitability assessment.
- Human review is mandatory.
- The AI cannot accept/reject a candidate.
