---
title: Actionable job stories from interview transcripts
category: User Research
tags:
  - user-research
  - jtbd
  - interviews
---
INPUTS
<provided_inputs>
- {{INTERVIEW_TRANSCRIPT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Actionable job stories from interview transcripts.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{INTERVIEW_TRANSCRIPT}}` to identify explicit and implicit user problems.
- Infer underlying needs from:
- Pain points, frustrations, inefficiencies.
- Context and background details.
- Goals, motivations, and desired outcomes.
- Workarounds and makeshift solutions.
- Generate job stories in this format:
- `When [situation], I want to [motivation], so I can [expected outcome].`
- Output only:
- A concise 2-3 sentence summary.
- A list of job stories grounded in transcript evidence.

FORMAT
Return exactly this structure:

<response>
<summary>
[Brief summary of your analysis]
</summary>
<job_stories>
<job_story>[Job story 1]</job_story>
<job_story>[Job story 2]</job_story>
[Additional <job_story> entries as needed]
</job_stories>
</response>

FAILURE
- `<response>`, `<summary>`, or `<job_stories>` is missing or malformed.
- Job stories do not follow `When... I want... so I can...` structure.
- Job stories are generic or not grounded in transcript-derived problems.
- Summary is missing or not within 2-3 sentences.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
