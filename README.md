# Project 3 - AI-Assisted Resume Screening Workflow

Independent GenAI Portfolio Project | Business Analysis | AI Workflow Design | Prompt Engineering | LLM Testing | Responsible AI

## Project Overview
This portfolio prototype simulates **TalentFlow**, a fictional recruitment operations organization that wants GenAI to organize candidate evidence before recruiter review.

The workflow extracts job requirements, extracts resume evidence, maps evidence to requirements, identifies matches/partial matches/gaps/unknowns, and produces a structured summary for human review.

**The AI does not make the final hiring decision.**

## Business Problem
Recruiters spend time manually extracting skills and experience, comparing them with job requirements, and preparing candidate summaries. The prototype evaluates whether an LLM can reduce repetitive analysis while preserving evidence grounding, responsible-AI controls, and human authority.

## Objective
Design and evaluate an AI-assisted workflow that extracts evidence from synthetic resumes, compares the evidence with job requirements, identifies matches and gaps, and produces an explainable summary for human review.

## AS-IS / TO-BE
**AS-IS:** Resume -> manual extraction -> manual comparison -> summary -> recruiter decision

**TO-BE:** JD + Resume -> requirement extraction -> resume extraction -> evidence mapping -> Match / Partial / Gap / Unknown -> structured summary -> HUMAN recruiter review -> final human decision

See `03-workflow/` for the diagram and control points.

## Requirements
See `02-requirements/` for functional requirements, AI-quality requirements, user stories and acceptance criteria.

## AI Workflow
1. Extract supported requirements from the JD.
2. Extract explicit candidate evidence from the resume.
3. Map each requirement to evidence.
4. Classify as Matched, Partial, Gap or Unknown.
5. Surface risks and unanswered questions.
6. Present a structured summary for human review.

## Prompt Versions
- **V1:** baseline task prompt
- **V2:** evidence grounding + anti-fabrication + uncertainty + responsible-AI guardrails
- **V3:** structured output + explicit human-review checklist

See `04-prompts/`.

## Synthetic Test Data
The project uses only fictional company and candidate data. See `05-test-data/`.

## Testing Approach
The test plan contains 22 scenarios covering normal matching, gaps, terminology, missing/vague evidence, hallucination, bias/fairness and decision boundaries. See `06-testing/`.

## Evaluation
Outputs are scored 1-5 across extraction accuracy, evidence grounding, hallucination control, matching quality, gap handling, bias control, explainability and human oversight. See `07-evaluation/`.

**Important:** actual scores, pass/fail results, defects and improvement claims must be based on real model executions.

## Responsible-AI Controls
- Human final decision
- Evidence grounding
- Unknown/uncertainty handling
- Irrelevant-attribute exclusion
- Synthetic data only
- No autonomous accept/reject behavior

## Current Execution Status
**Project pack status:** Ready for hands-on execution.

**Evidence status:** Actual LLM outputs, screenshots, test results, evaluation scores and findings must be populated from your real runs. Blank/pending fields are intentional and prevent fabricated portfolio evidence.

## Tools
Record the actual tools/models used during execution in the prompt execution logs and README update section.

## Repository Structure
```text
01-business/
02-requirements/
03-workflow/
04-prompts/
05-test-data/
06-testing/
07-evaluation/
08-case-study/
screenshots/
learning-notes.md
README.md
```

## Disclaimer
This is an independent portfolio simulation, not employment or a production recruitment system. It does not claim production accuracy, legal compliance, or real hiring outcomes.
