---
title: Onboarding flow optimization from product data to user success
category: Business Analysis
tags:
  - pm
  - onboarding
  - growth
  - user-success
  - business-analysis
---
INPUTS
<provided_inputs>
- {{PRODUCT_DESCRIPTION}}
- {{TARGET_AUDIENCE}}
- {{CURRENT_ONBOARDING_PROCESS}}
</provided_inputs>

GOAL
Design an actionable onboarding optimization plan that moves users from initial state to first meaningful success faster and more reliably.
Success metric:
- Clearly defines user transformation and first meaningful success step.
- Maps desired outcomes to current blockers and practical small-win interventions.
- Proposes progress/momentum mechanics that can be directly used in a PRD or design brief.
- Follows the required output schema exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, section logic, or actionable recommendation details.
- Keep recommendations grounded in `PRODUCT_DESCRIPTION`, `TARGET_AUDIENCE`, and `CURRENT_ONBOARDING_PROCESS`.
- Perform this sequence:
  1. Define transformation:
     - user before state,
     - user after state,
     - smallest step to experience meaningful progress.
  2. Map dream to reality:
     - desired end state,
     - current blockers,
     - confidence-building small wins.
  3. Design progress (not just features):
     - visible progress signals,
     - small-win celebrations,
     - obvious next-step mechanics,
     - momentum loops.
- Recommendations must be concrete enough to be implemented in a PRD/design brief.
- Explicitly label assumptions where data/process detail is missing.

FORMAT
Return exactly this structure:

<onboarding_improvement_plan>
<transformation_definition>
[Your analysis and recommendations for step 1]
</transformation_definition>

<dream_to_reality_mapping>
[Your analysis and recommendations for step 2]
</dream_to_reality_mapping>

<progress_design>
[Your analysis and recommendations for step 3]
</progress_design>

<conclusion>
[Summarize the key points of your improvement plan and highlight the most impactful changes]
</conclusion>
</onboarding_improvement_plan>

FAILURE
- Required schema is missing, malformed, or incomplete.
- Any of the 3 core steps (transformation, dream-to-reality mapping, progress design) is missing or shallow.
- Recommendations are generic, not tied to provided product/audience/process context.
- Output lacks concrete actions suitable for a PRD/design brief.
- Assumptions are used but not explicitly stated.
