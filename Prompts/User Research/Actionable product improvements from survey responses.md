---
title: Actionable product improvements from survey responses
category: User Research
tags:
  - user-research
  - surveys
  - insights
---
INPUTS
<provided_inputs>
- {{SURVEY_RESPONSES}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Actionable product improvements from survey responses.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{SURVEY_RESPONSES}}` to identify recurring themes and distinct user pain points.
- For each pain point, include:
- At least two supporting quotes from different responses where possible.
- One or more concrete, actionable improvement items.
- Ensure findings are evidence-based, specific, and focused on improving product/service/process outcomes.
- Identify multiple themes when the dataset supports it.

FORMAT
Return exactly this structure:

<analysis>
<theme>
<pain_point>[Describe the pain point]</pain_point>
<supporting_quotes>
- "[Relevant quote]" (Response #X)
- "[Relevant quote]" (Response #Y)
</supporting_quotes>
<action_items>
- [Action item 1]
- [Action item 2]
</action_items>
</theme>
[Repeat `<theme>` for each identified theme]
</analysis>

FAILURE
- `<analysis>` or `<theme>` schema is missing, malformed, or materially incomplete.
- Pain points are generic and not supported by response evidence.
- Any theme lacks at least two supporting quotes.
- Action items are vague, non-actionable, or not linked to the stated pain point.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
