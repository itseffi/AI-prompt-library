---
title: Startup ideas from user responses
category: User Research
tags:
  - user-research
  - ideation
  - startup
---
INPUTS
<provided_inputs>
- `{{USER_RESPONSES}}`: User answers describing goals, workflow, pain points, constraints, and attempted solutions.
</provided_inputs>

GOAL
Generate startup software product ideas grounded in user responses and priced at clear bargain-value for approximately $30/month.
Success metric:
- Ideas directly map to concrete pains/opportunities in the provided responses.
- Output includes exactly ten distinct ideas with clear value propositions.
- Each idea is concise, specific, and formatted exactly as required.

CONSTRAINTS
- Use only `{{USER_RESPONSES}}`; if information is missing, state assumptions briefly before the ideas.
- Analyze responses for:
- User's overall goal.
- Process steps and current stage.
- Workflow location of the problem.
- Time/money-heavy pain points.
- Problem frequency.
- Previously attempted solutions.
- Propose only software product concepts (conceptual feasibility is acceptable).
- Generate diverse ideas (avoid minor variants of the same concept).
- Each idea must include:
- A unique number.
- A catchy product name.
- A 40-80 word description.
- Each description must explain how the idea reduces friction, time, cost, or risk in the user's workflow.

FORMAT
Return exactly ten separate `<idea>` blocks in this pattern:

<idea>
[Number]. [Name]: [Description in 40-80 words]
</idea>

Rules:
- Numbering must run from `1` to `10` with no gaps or duplicates.
- Each `<idea>` block must be a separate paragraph.

FAILURE
- Fewer or more than 10 ideas are returned.
- Any idea is missing number, name, or description.
- Any description is outside 40-80 words.
- Ideas are generic, repetitive, or not grounded in `{{USER_RESPONSES}}`.
- Output does not use the required `<idea>` block format.
- Assumptions are needed but not explicitly stated.
