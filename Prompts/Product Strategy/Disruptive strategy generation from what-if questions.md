---
title: Disruptive strategy generation from what-if questions
category: Product Strategy
tags:
  - strategy
  - counter-positioning
  - brainstorming
  - disruption
  - competitive-analysis
---
INPUTS
<provided_inputs>
- {{COMPANY_OR_PRODUCT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Disruptive strategy generation from what-if questions.
Success metric:
- Produces a grounded analysis of the incumbent and a diverse set of counter-positioning "what if" questions.
- Generates 20–30 specific, actionable questions across multiple disruption dimensions.
- Keeps outputs tied to the company's business model and customer assumptions.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{COMPANY_OR_PRODUCT}}`; if critical details are missing, state assumptions explicitly.
- Start with a brief, grounded analysis of how the incumbent makes money, core product elements, and strategic posture.
- Generate 20–30 "what if" questions that are specific and actionable.
- Ensure diversity across at least these dimensions:
  - technology,
  - business model,
  - customer experience,
  - market expansion,
  - sustainability,
  - regulatory changes.
- Questions must challenge core assumptions and suggest plausible counter-positioning angles.

FORMAT
Return exactly this structure:

<reasoning>
[Analysis of the company/product and what makes it successful]
</reasoning>

<what_if_questions>
1. [Your first "what if" question]
2. [Your second "what if" question]
...
[Continue until you have 20–30 questions]
</what_if_questions>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 20 or more than 30 questions are provided.
- Questions are generic, repetitive, or not tied to the company/product context.
- Diversity across the required dimensions is missing.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
