---
title: Actionable user research decisions from project insights
category: User Research
tags:
  - user-research
  - decision-making
  - frameworks
---
INPUTS
<provided_inputs>
- {{PROJECT_DESCRIPTION}}
- {{DEVELOPMENT_STAGE}}
- {{EVIDENCE_NEEDS}}
- {{SPLASH_ZONE_IMPACT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Actionable user research decisions from project insights.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Apply the Reforge-style user insights decision framing to:
- `{{PROJECT_DESCRIPTION}}`
- `{{DEVELOPMENT_STAGE}}`
- `{{EVIDENCE_NEEDS}}`
- `{{SPLASH_ZONE_IMPACT}}`
- Produce a specific research decision description framed as a question.
- Ensure the decision question is:
- Concrete and visceral (not abstract).
- Specific to user, context, behavior, and decision consequence.
- Aligned to stage-appropriate evidence needs.
- Scoped to the stated splash-zone/impact.
- Include assumptions explicitly if required context is missing.

FORMAT
Return exactly this structure:

<scratchpad>
[Use this space to think through and refine your decision description]
</scratchpad>

<decision_description>
[Write your final decision description here]
</decision_description>

FAILURE
- `<scratchpad>` or `<decision_description>` is missing, malformed, or materially incomplete.
- Decision description is not phrased as a researchable question.
- Language is vague/abstract and not specific to stage, evidence needs, or splash-zone impact.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
