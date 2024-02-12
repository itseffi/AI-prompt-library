---
title: "Structured requirements from design assets"
category: "Business Analysis"
tags:
  - pm
  - business-analysis
  - requirements
  - design
---
INPUTS
<provided_inputs>
- {{IMAGE}}
</provided_inputs>

GOAL
Translate `IMAGE` design assets into actionable, testable product requirements and acceptance criteria.
Success metric:
- Produces clear, numbered user stories/requirements covering key flows and behaviors shown or implied in the design.
- Provides detailed acceptance criteria mapped to each requirement.
- Keeps requirements implementation-agnostic (focus on "what", not "how").
- Follows the required output schema exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip analysis of visual structure, information hierarchy, interactions, states, and implied business rules.
- Number each requirement/story and keep it measurable and implementation-agnostic.
- Acceptance criteria must map to requirements explicitly (by requirement number/id).
- Include inferred assumptions only when necessary and label them clearly.
- Do not include internal reasoning tags like `<scratchpad>` in final output.

FORMAT
Return exactly this structure:

<requirements>
<user_stories>
[List numbered user stories or requirements here]
</user_stories>

<acceptance_criteria>
[List detailed acceptance criteria for each user story or requirement here]
</acceptance_criteria>
</requirements>

FAILURE
- Required schema is missing or malformed.
- Requirements are generic, non-measurable, or not grounded in the design asset.
- Acceptance criteria are missing, vague, or not mapped to requirements.
- Output contains implementation-detail overreach instead of product requirements.
- Assumptions are used but not explicitly stated.
