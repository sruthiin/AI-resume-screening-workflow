# Learning Notes

## AI-assisted workflow
An AI-assisted workflow places an LLM inside a defined business process with explicit inputs, outputs, controls and human responsibilities. The model supports an activity rather than owning the final business decision.

## Human-in-the-loop
Human review is needed because candidate context can be incomplete, ambiguous and consequential. In this prototype, the AI organizes evidence and uncertainty; the human reviews the analysis and owns the final decision.

## Information extraction
Information extraction converts unstructured text such as a JD or resume into structured facts that can be compared. A key quality rule is to extract what is present without creating new facts.

## Skill matching
Skill matching is a comparison between stated job requirements and candidate evidence. Semantic similarity can help identify related terminology, but similarity alone is not proof that a specific tool or level of expertise is present.

## False positive vs false negative
A false positive match occurs when the AI claims a requirement is supported when the evidence does not support it. A false negative occurs when legitimate evidence is missed or treated as unsupported.

## Evidence grounding
Evidence grounding means important claims can be traced back to text supplied in the prompt. This helps the human reviewer verify the model output.

## Hallucinated qualifications
An LLM can produce plausible-sounding facts that are not present in the source text. Recruitment analysis must explicitly prohibit invented skills, employers, durations, certifications, achievements and metrics.

## Irrelevant personal data and bias
Personal attributes that are not job requirements can become leakage features. Paired synthetic resumes provide a controlled way to check whether changing irrelevant details changes the job-related assessment.

## Missing evidence is not proven absence
A resume that does not mention a skill does not prove the candidate lacks it. The safer workflow uses Gap or Unknown according to the available evidence and keeps human review in the loop.

## Autonomous decisions
A resume analysis assistant should not accept or reject a candidate in this portfolio prototype. The output should instead provide evidence, uncertainty, risks and questions for human review.
