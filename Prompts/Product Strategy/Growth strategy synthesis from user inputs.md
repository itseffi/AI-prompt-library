---
title: Growth strategy synthesis from user inputs
category: Product Strategy
tags:
  - growth
  - strategy
  - experimentation
  - metrics
  - distribution
---
INPUTS
<provided_inputs>
- {{USER_INPUTS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Growth strategy synthesis from user inputs.
Success metric:
- Produces a complete growth strategy across model, constraints, horizon, method, principle, and catalyst.
- Grounds all recommendations in the provided user inputs.
- Outputs actionable, testable recommendations and a concise summary.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{USER_INPUTS}}`; if critical data is missing, state assumptions explicitly.
- Address each required section: model, constraint, horizon, method, principle, catalyst, summary.
- Keep recommendations actionable and testable; avoid generic advice.
- If quantitative data is present, reference it; if not, use qualitative reasoning and label assumptions.

FORMAT
Return exactly this structure:

<growth_strategy>
<growth_model>
[Provide a detailed description of the growth model]
</growth_model>

<growth_constraint>
[Identify and explain the main growth constraints]
</growth_constraint>

<growth_horizon>
[Analyze the growth horizon and potential limitations]
</growth_horizon>

<growth_method>
[Propose specific methods to address constraints and extend the growth horizon]
</growth_method>

<growth_principle>
[Develop a guiding principle for aligning the organization]
</growth_principle>

<growth_catalyst>
[Identify and explain any growth catalysts]
</growth_catalyst>

<summary>
[Provide a brief summary of the overall growth strategy]
</summary>
</growth_strategy>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Recommendations are not tied to the provided inputs.
- Growth method lacks actionable steps.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
