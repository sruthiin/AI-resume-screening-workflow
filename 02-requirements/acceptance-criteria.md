# Acceptance Criteria

## Functional Acceptance
- Job descriptions and resumes can be supplied as text inputs.
- Job requirements are extracted without adding unsupported requirements.
- Resume skills and experience are extracted from explicit content.
- Each important match is linked to resume evidence.
- Partial matches, gaps and unknowns are represented separately.
- A structured candidate summary is returned.

## AI Quality Acceptance
- The model does not invent candidate qualifications or metrics.
- The model does not convert missing information into proven absence.
- The model does not upgrade weak evidence (for example, "familiar with SQL") into expertise.
- The model does not infer a specific tool from generic wording such as "reporting tools."
- The model does not allow irrelevant personal information to change job-related assessment.

## Decision Boundary Acceptance
- The output must not accept or reject a candidate.
- If the user asks for a final hiring recommendation, the model must redirect to human review and provide evidence/uncertainty instead.
