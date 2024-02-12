---
title: OKR planning from vision statements
category: Product Strategy
tags:
  - okrs
  - strategy
  - goal-setting
  - product-management
  - execution
  - prioritization
---
INPUTS
<provided_inputs>
- {{VISION_STATEMENT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: OKR planning from vision statements.
Success metric:
- Converts the vision into 3–5 key areas with quarterly objectives and measurable key results.
- Ensures key results are quantitative and tied to product milestones.
- Includes a clear explanation of alignment back to the vision.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{VISION_STATEMENT}}`; if context is missing, state assumptions explicitly.
- Create 3–5 key areas; each has 1–2 objectives.
- Each objective must have 2–4 quantitative key results tied to product milestones.
- Keep OKRs specific to the vision and industry; avoid generic templates.
- Include an explanation mapping each key area to the vision.

FORMAT
Return exactly this structure:

<okrs>
Key Area 1:
Objective 1:
- Key Result 1
- Key Result 2
- Key Result 3

Key Area 2:
Objective 1:
- Key Result 1
- Key Result 2
- Key Result 3

Objective 2:
- Key Result 1
- Key Result 2
- Key Result 3

(Continue for all key areas, objectives, and key results)
</okrs>

<explanation>
[Explain how each key area and its OKRs map back to the vision statement]
</explanation>

FAILURE
- `<okrs>` or `<explanation>` is missing, malformed, or incomplete.
- Fewer than 3 or more than 5 key areas are provided.
- Objectives or key results are missing or not within required counts.
- Key results are not quantitative or not tied to product milestones.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
