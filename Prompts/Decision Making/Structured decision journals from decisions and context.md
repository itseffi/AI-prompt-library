---
title: "Structured decision journals from decisions and context"
category: "Decision Making"
tags:
  - pm
  - decision-making
  - journaling
  - forecasting
  - base-rates
---
INPUTS
<provided_inputs>
- {{DECISION}}
- {{CONTEXT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Structured decision journals from decisions and context".
Success metric:
- Produces a complete decision journal with all required sections filled from provided context.
- Probability estimates are coherent and sum to 100%.
- Quit conditions are measurable and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{DECISION}}` and `{{CONTEXT}}`; if information is missing, state assumptions explicitly.
- Generate 3-5 expected outcomes spanning best-case to worst-case and covering short-term and long-term effects.
- Provide one probability for each expected outcome; probabilities must total exactly 100%.
- Provide 3-5 key assumptions that materially affect outcome validity.
- Provide relevant base rates/statistics tied to this decision type; if unavailable, provide directional proxies and label as assumptions.
- Provide 2-3 measurable quit conditions with clear trigger thresholds.
- Keep `<actual_results>` intentionally blank for future updates.

FORMAT
Return exactly this structure:

<decision_journal>
<expected_outcomes>
1. [Outcome]
2. [Outcome]
3. [Outcome]
[Optional 4th and 5th outcome]
</expected_outcomes>

<probability_estimates>
1. [Outcome 1] - [X%]
2. [Outcome 2] - [Y%]
3. [Outcome 3] - [Z%]
[Optional 4th and 5th probability]
Total: 100%
</probability_estimates>

<key_assumptions>
1. [Assumption]
2. [Assumption]
3. [Assumption]
[Optional 4th and 5th assumption]
</key_assumptions>

<base_rates>
1. [Base rate/statistic + source context or rationale]
2. [Base rate/statistic + source context or rationale]
[Optional additional base rates]
</base_rates>

<quit_conditions>
1. [Condition + measurable threshold]
2. [Condition + measurable threshold]
[Optional 3rd condition]
</quit_conditions>

<actual_results>
</actual_results>
</decision_journal>

FAILURE
- Any required section in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 3 or more than 5 expected outcomes.
- Probability estimates do not map to outcomes or do not total 100%.
- Fewer than 3 key assumptions or fewer than 2 quit conditions.
- Quit conditions are not measurable.
- Claims are generic or not grounded in provided inputs.
- `<actual_results>` is pre-filled with outcome claims.
- Assumptions are used but not explicitly stated.
