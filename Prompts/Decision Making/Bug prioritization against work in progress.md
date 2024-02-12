---
title: "Bug prioritization against work in progress"
category: "Decision Making"
tags:
  - pm
  - decision-making
  - prioritization
  - bugs
  - triage
---
INPUTS
<provided_inputs>
- {{BUG_DESCRIPTION}}
- {{CURRENT_WORK}}
- {{PLANNED_WORK}}
</provided_inputs>

GOAL
Determine whether a reported bug should take priority over current and planned work, then provide a triage decision.
Success metric:
- Provides clear reasoning and YES/NO decision for both prioritization questions.
- Final decision is logically consistent with those two answers.
- Uses only provided bug/current/planned work context.
- Follows the required output schema exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip either required question:
  1. Is this bug more important than current work?
  2. Is this bug more important than planned next work?
- For each question, include concise reasoning before the YES/NO answer.
- Apply decision rule strictly:
  - If both answers are `NO` -> `Do not prioritize fixing this bug now`.
  - If either answer is `YES` -> `Proceed to further classification`.
- Keep reasoning grounded in bug impact, user/business risk, and delivery tradeoffs from provided context.

FORMAT
Return exactly this structure:

<question1>
Reasoning: [Your reasoning here]
Answer: [YES/NO]
</question1>

<question2>
Reasoning: [Your reasoning here]
Answer: [YES/NO]
</question2>

<decision>
[Your decision here: either "Do not prioritize fixing this bug now" or "Proceed to further classification"]
</decision>

FAILURE
- Missing `<question1>`, `<question2>`, or `<decision>` section.
- Missing reasoning or missing YES/NO answer for either question.
- Final decision contradicts the required decision rule.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
