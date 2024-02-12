---
title: Product assumptions from core strategy inputs
category: User Research
tags:
  - user-research
  - assumptions
  - product-strategy
---
INPUTS
<provided_inputs>
- `{{PRODUCT_DESCRIPTION}}`: Product concept, scope, and intended value.
- `{{CORE_PROBLEM}}`: Core user/business problem the product addresses.
- `{{TARGET_USER}}`: Primary target user segment(s).
</provided_inputs>

GOAL
Produce a rigorous, testable assumption set underlying the product strategy across desirability, feasibility, viability, and usability.
Success metric:
- Assumptions are specific, falsifiable, and impact-aware.
- Assumptions are non-duplicative across categories and grounded in provided inputs.
- Output follows the required plain-text structure exactly.

CONSTRAINTS
- Use only provided inputs and disciplined inference.
- If any input is missing or vague, proceed with prudent defaults and note gaps only in `SUMMARY`.
- Do not use XML, HTML, angle-bracket tags, or code fences in the model output.
- Return only the required sections in the required order.
- Create exactly four assumption categories in this order:
- Desirability Assumptions
- Feasibility Assumptions
- Viability Assumptions
- Usability Assumptions
- Each category must contain at least 5 assumptions.
- Each assumption must be one numbered item with exactly two labeled lines:
- `Statement:` starts with `We believe that...`, is one idea only, specific/falsifiable, and max 35 words.
- `Impact if wrong:` one concise sentence describing concrete consequence (adoption, cost, timeline, risk, or strategy).
- Avoid repeating the same assumption across categories.
- Include measurable thresholds, segments, conditions, or timeframes where possible.
- Reflect relevant product-strategy realities (for example: compliance, integrations, data quality, reliability/SLOs, scalability, CAC/LTV, retention, pricing power, partner economics).

FORMAT
Return plain text only, using exactly this section structure and order:

ASSUMPTIONS LIST
Desirability Assumptions
1.
Statement: We believe that ...
Impact if wrong: ...

2.
Statement: We believe that ...
Impact if wrong: ...

[at least 5 items]

Feasibility Assumptions
1.
Statement: We believe that ...
Impact if wrong: ...

[at least 5 items]

Viability Assumptions
1.
Statement: We believe that ...
Impact if wrong: ...

[at least 5 items]

Usability Assumptions
1.
Statement: We believe that ...
Impact if wrong: ...

[at least 5 items]

SUMMARY
- Key risk themes across the four categories.
- Most critical assumptions to validate first.
- Any missing/vague input gaps and explicit defaults used.

FAILURE
- Output contains anything other than `ASSUMPTIONS LIST` followed by `SUMMARY`.
- Any category is missing, out of order, or has fewer than 5 assumptions.
- Any assumption is missing either `Statement:` or `Impact if wrong:`.
- Any `Statement:` does not start with `We believe that...`, exceeds 35 words, or contains multiple claims.
- Assumptions are generic, non-falsifiable, duplicated across categories, or not grounded in provided inputs.
- Missing/vague input handling is not explicitly documented in `SUMMARY`.
- Output includes XML/HTML tags, angle-bracket tags, or code fences.
