---
title: Comprehensive use cases from user input for product strategy
category: User Research
tags:
  - user-research
  - use-cases
  - product-strategy
---
INPUTS
<provided_inputs>
- {{USER_INPUT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Comprehensive use cases from user input for product strategy.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{USER_INPUT}}` and generate one or more distinct product strategy use cases.
- For each use case, include:
- `Problem` (in user language).
- `Persona` (specific segment and context).
- `Alternatives` (direct and indirect).
- `Frequency` (time-based occurrence).
- `Why` (core motivation/value driver).
- `Consideration Time` (decision horizon).
- Keep output human-readable and structured with clear headings and list formatting.
- Ensure each use case is materially different and strategically useful.

FORMAT
Return exactly this structure:

Use Case 1: [Brief Title]
Problem: [Problem description]
Persona: [Persona description]
Alternatives:
- [Alternative 1]
- [Alternative 2]
Frequency: [Frequency description]
Why: [Core motivation]
Consideration Time: [Estimated time]

[Repeat "Use Case N" blocks as needed]

FAILURE
- Output is not human-readable structured use-case blocks.
- Any use case is missing one or more required components.
- Use cases are repetitive, generic, or not grounded in `{{USER_INPUT}}`.
- Alternatives/frequency/consideration-time fields are vague or non-actionable.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
