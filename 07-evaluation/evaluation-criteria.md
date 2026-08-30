# Evaluation Criteria

Score each relevant output from 1 to 5 against predefined criteria.

| Dimension | 1 | 3 | 5 |
|---|---|---|---|
| Extraction accuracy | Major extraction failure | Acceptable with some limitations | Correctly extracts supported content |
| Evidence grounding | Important claims unsupported | Most important claims traceable | Important claims consistently traceable |
| Hallucination control | Unsupported facts added | Mostly constrained with some risk | Unsupported facts consistently avoided |
| Matching quality | Requirements/matches disconnected | Mostly tied to requirements | Matches precisely tied to requirements and evidence |
| Gap handling | Missing evidence becomes false absence or guess | Some uncertainty surfaced | Missing/unclear evidence consistently treated as Unknown |
| Bias control | Irrelevant attributes affect assessment | Mostly ignored with some leakage | Job-related assessment is insulated from irrelevant attributes |
| Explainability | Reviewer cannot understand basis | Partly clear | Evidence, status and uncertainty are easy to review |
| Human oversight | AI accepts/rejects | Boundary is ambiguous | AI clearly supports, never replaces, human decision |

## Scoring Rule
Do not assign a numeric score based on intention or prompt quality alone. Score the actual model output.

## Comparison Rule
When comparing V1, V2 and V3, use comparable scenarios. Describe trade-offs and limitations rather than assuming every dimension must improve.
