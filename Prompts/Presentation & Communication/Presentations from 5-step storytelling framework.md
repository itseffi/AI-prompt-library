---
title: Presentations from 5-step storytelling framework
category: Presentation & Communication
tags:
  - presentations
  - storytelling
  - product-management
  - communication
---
INPUTS
<provided_inputs>
- {{PRESENTATION_TOPIC}}
- {{CURRENT_STEP}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Presentations from 5-step storytelling framework.
Success metric:
- Provides concrete guidance tailored to the specified current step in the 5-step process.
- Integrates storytelling principles into step-specific presentation advice.
- Ends with a clear request for user progress/questions to continue iteration.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRESENTATION_TOPIC}}` and `{{CURRENT_STEP}}`; if context is missing, state assumptions explicitly.
- Tailor guidance to exactly one of these steps:
  1. Paper outline
  2. Paper storyboard
  3. Headlines first
  4. Fill them in
  5. Practice
- Guidance must include concrete next actions for the current step (not generic advice for all steps).
- Integrate storytelling principles:
  - hook/call,
  - trial/tribulations,
  - transformation/climax,
  - return/call-to-action,
  - tradeoffs/challenges.
- Use practical language and suggest artifacts/checklists relevant to the selected step.
- End by asking the user to share progress or questions.

FORMAT
Return exactly this structure:

<guidance>
[Step-specific instructions for `{{CURRENT_STEP}}`, tailored to `{{PRESENTATION_TOPIC}}`, including storytelling integration]
</guidance>

<request>
[Ask the user to share progress, draft output, or questions for the current step]
</request>

FAILURE
- `<guidance>` or `<request>` is missing, malformed, or empty.
- Guidance is not specific to the declared `{{CURRENT_STEP}}`.
- Guidance omits storytelling principles or does not relate them to the step.
- Request does not explicitly ask for user progress/questions.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
