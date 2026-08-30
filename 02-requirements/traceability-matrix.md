# Requirements Traceability Matrix

| Requirement / Story | Workflow Step | Prompt Control | Test Coverage | Evidence Artifact |
|---|---|---|---|---|
| FR-003 Resume skills extraction | Resume evidence extraction | Explicit-information-only rule | TC-001 to TC-004, TC-012 to TC-013 | Actual model output |
| FR-005 JD requirement extraction | Requirement extraction | Supplied-JD-only rule | TC-001, TC-003 | Actual model output |
| FR-006 Evidence-to-requirement comparison | Evidence mapping | Evidence required for matches | TC-001 to TC-011 | Actual mapping |
| FR-007 Gap identification | Match classification | Unknown / insufficient evidence | TC-005 to TC-008, TC-012 to TC-014 | Actual output |
| AIR-001 Source grounding | All analysis | Use only supplied information | TC-015 to TC-017 | Actual output + screenshot |
| AIR-002 No invented candidate facts | All analysis | Anti-fabrication rule | TC-015 to TC-017 | Defect log if failed |
| AIR-003 Evidence vs assumptions | Evidence mapping | Evidence column + uncertainty | TC-009 to TC-014 | Evaluation sheet |
| AIR-004 Missing information handling | Classification | Unknown instead of guessing | TC-005 to TC-008, TC-014 | Actual output |
| AIR-005 Evidence for claims | Evidence mapping | Every important match cites evidence | TC-001 to TC-011 | Match-evidence screenshot |
| AIR-006 Irrelevant personal attributes excluded | Matching/review | Attribute exclusion rule | TC-018 to TC-020 | Paired fairness screenshots |
| US-006 Human review | Human checkpoint | Explicit no-final-decision rule | TC-021 to TC-022 | Human-review screenshot |
