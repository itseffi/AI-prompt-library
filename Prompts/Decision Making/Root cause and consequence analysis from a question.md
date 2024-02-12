---
title: "Root cause and consequence analysis from a question"
category: "Decision Making"
tags:
  - pm
  - decision-making
  - analysis
  - root-causes
  - reasoning
---
INPUTS
<provided_inputs>
- {{INITIAL_QUESTION}}
</provided_inputs>

GOAL
Identify plausible root causes and downstream consequences of `INITIAL_QUESTION` using recursive why-analysis and first-principles reasoning.
Success metric:
- Performs a deep why-chain (target depth: at least 5 levels or until a defensible root cause boundary).
- Explores consequence orders from first through fifth (positive and negative where plausible).
- Distinguishes assumptions from inferred facts and flags logic gaps.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis layers:
  1. Recursive why-analysis.
  2. Consequence chain (1st to 5th order).
  3. First-principles reconstruction.
- For why-analysis, explore parallel branches when multiple plausible causes emerge.
- For consequence analysis, include both upside and downside outcomes when credible.
- Keep reasoning neutral and explicit; avoid unsupported certainty.
- Clearly label assumptions and unknowns.

FORMAT
Return exactly this structure:

<analysis>
<root_causes>
[List your "Why?" questions and answers here, showing the progression to the root cause(s)]
</root_causes>

<consequences>
[Describe the potential consequences here, from first-order to fifth-order]
</consequences>

<first_principles>
[Present your first principles analysis here, including fundamental truths, questioned assumptions, and any identified gaps]
</first_principles>

<conclusion>
[Summarize your key findings and insights]
</conclusion>
</analysis>

FAILURE
- Required schema is missing or malformed.
- Why-analysis is shallow (no meaningful depth/branching) or lacks root-cause rationale.
- Consequence analysis does not cover first through fifth order.
- First-principles section does not separate assumptions from fundamentals.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
