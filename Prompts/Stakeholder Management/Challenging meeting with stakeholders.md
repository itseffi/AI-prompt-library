---
title: Challenging meeting with stakeholders
category: Stakeholder Management
tags:
  - stakeholders
  - meeting-prep
  - risk-management
---
INPUTS
<provided_inputs>
- {{GOAL_OR_CONTEXT}}
- {{STAKEHOLDERS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Challenging meeting with stakeholders.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Generate at least 20 challenging stakeholder questions based on `{{GOAL_OR_CONTEXT}}` and `{{STAKEHOLDERS}}`.
- Cover financials, resources, timeline, risks, market, competition, feasibility, UX, ethics, sustainability, team capability, past performance, strategy alignment, compliance, and scalability.
- Make questions rigorous and probing; avoid generic filler.

FORMAT
Return exactly this structure:

<question_list>
1. [First question]
2. [Second question]
3. [Third question]
...
</question_list>

FAILURE
- `<question_list>` is missing, malformed, or has fewer than 20 questions.
- Questions are generic, repetitive, or not tied to the provided context.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
