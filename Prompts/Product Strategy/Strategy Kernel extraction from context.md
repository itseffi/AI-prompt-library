---
title: Strategy Kernel extraction from context
category: Product Strategy
tags:
  - strategy
  - product-management
  - diagnosis
  - context
---
INPUTS
<provided_inputs>
- {{PRODUCT_MANAGER_INPUT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Strategy Kernel extraction from context.
Success metric:
- Extracts explicit, implied, and missing strategic context with clear gaps and next steps.
- Flags risks/anti-patterns and prioritizes follow-up questions.
- Produces a structured assessment aligned to the Strategy Kernel Canvas sections.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT_MANAGER_INPUT}}`; if key context is missing, state assumptions explicitly.
- Extract explicit, implied, and missing information across History, Diagnosis, and Guiding Policy.
- Flag anti-patterns when supported by the input.
- Provide 3–5 prioritized clarification questions if critical gaps remain.
- Keep output structured and decision-ready; no fluff.

FORMAT
Return exactly this structure:

context_assessment:
  completeness_score: [0-100]
  confidence_level: [high/medium/low]

  explicit_information:
    - [Clearly stated items]

  implied_information:
    - [Reasonable inferences]

  critical_gaps:
    - gap: [description]
      why_critical: [explanation]
      how_to_obtain: [suggested action]

  red_flags:
    - [Potential derailers]

  recommended_focus_areas:
    - [Where to focus effort]

  stakeholder_map:
    - name/role: [name or role]
      influence: [high/medium/low]
      alignment: [aligned/neutral/opposed/unknown]

  next_steps:
    immediate:
      - [Next 24 hours]
    week_one:
      - [First week actions]

clarifying_questions:
  - "[CRITICAL] [Question] - Why this matters: [explanation]"
  - "[IMPORTANT] [Question] - Why this matters: [explanation]"
  - "[USEFUL] [Question] - Why this matters: [explanation]"

FAILURE
- Output is missing `context_assessment` or `clarifying_questions`.
- Completeness score or confidence level is missing.
- Critical gaps are missing when evidence is insufficient.
- Clarifying questions are not prioritized or fewer than 3 when needed.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
