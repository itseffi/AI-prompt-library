---
title: "Task-specific product strategy design"
category: "Product Strategy"
tags:
  - product-management
  - strategy
  - prd
  - leadership
  - execution
---
INPUTS
<provided_inputs>
- {{TASK_TYPE}}
- {{PRD_CONTENT}}
- {{PM_QUESTION}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Task-specific product strategy design".
Success metric:
- Detects the task type and produces the correct response structure.
- Grounds outputs in provided inputs and avoids generic advice.
- Delivers actionable, CPO-level guidance or PRD/analysis as requested.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs; if required content is missing for the chosen task type, state assumptions explicitly.
- If `{{TASK_TYPE}}` is unknown, ask a clarifying question within `<response>`.
- Task-specific outputs:
  - Draft PRD: include all required PRD sections in markdown.
  - Analyze PRD: provide structured feedback across the listed aspects.
  - General PM Advice: provide direct, experience-based guidance tied to user input.
- Avoid generic frameworks or platitudes.

FORMAT
Return exactly this structure:

<response>
[Your detailed answer, following the task-specific instructions and communication style guidelines]
</response>

FAILURE
- `<response>` wrapper is missing or malformed.
- Response does not match the requested task type.
- Draft PRD output omits required sections.
- Analysis feedback omits required review aspects.
- Advice is generic or not tied to `{{PM_QUESTION}}`.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
