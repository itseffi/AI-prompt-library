---
title: Framework application to product challenges from user input
category: Product Strategy
tags:
  - product-strategy
  - frameworks
  - decision-making
  - coaching
---
INPUTS
<provided_inputs>
- {{FRAMEWORK}}
- {{USER_INPUT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Framework application to product challenges from user input.
Success metric:
- Asks targeted questions when key context is missing.
- Applies the provided framework precisely to the user’s situation.
- Produces actionable advice and a clear recommendation when sufficient context exists.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{FRAMEWORK}}` and `{{USER_INPUT}}`; if key context is missing, ask targeted questions first.
- Do not summarize the framework back to the user.
- When asking for more information, use `<question>` tags only.
- When providing guidance, use `<advice>` tags only.
- When providing a final recommendation, use `<recommendation>` tags only.
- Keep advice specific and grounded in the user’s context; avoid generic PM guidance.

FORMAT
Return exactly this structure:

<question>
[Targeted questions needed to apply the framework]
</question>

<advice>
[Framework-applied guidance once sufficient context exists]
</advice>

<recommendation>
[Final recommendation when enough context exists]
</recommendation>

FAILURE
- Required tags are missing or malformed.
- Output includes framework summary instead of application.
- Advice is generic or not tied to the user input.
- Recommendation is provided without sufficient context.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
