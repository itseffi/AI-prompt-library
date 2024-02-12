---
title: Ideas for affordances and signifiers based on a design problem
category: Design & Prototyping
tags:
  - ux
  - interaction-design
  - affordances
  - usability
---
INPUTS
<provided_inputs>
- {{DESIGN_CHALLENGE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Ideas for affordances and signifiers based on a design problem.
Success metric:
- Identifies key user interactions in the design challenge before proposing ideas.
- Produces at least 5 concrete ideas each for affordances, perceived affordances, and signifiers.
- Each idea includes a brief explanation tied to the challenge and UX impact.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{DESIGN_CHALLENGE}}`; if context is incomplete, state assumptions explicitly.
- Start with a brief interaction analysis identifying main user functions/tasks.
- Generate at least 5 ideas in each category: affordances, perceived affordances, signifiers.
- For every idea, include a short explanation linking:
  - the specific challenge friction/opportunity,
  - how the idea guides user action or perception,
  - expected UX improvement.
- Keep ideas practical, non-generic, and directly relevant to the described product context.

FORMAT
Return exactly this structure:

<ideas>
<interaction_analysis>
[Main user interactions/functions required by the challenge]
</interaction_analysis>

<affordances>
1. [Affordance idea] - [Brief explanation]
2. [Affordance idea] - [Brief explanation]
3. [Affordance idea] - [Brief explanation]
4. [Affordance idea] - [Brief explanation]
5. [Affordance idea] - [Brief explanation]
[Optional additional ideas]
</affordances>

<perceived_affordances>
1. [Perceived affordance idea] - [Brief explanation]
2. [Perceived affordance idea] - [Brief explanation]
3. [Perceived affordance idea] - [Brief explanation]
4. [Perceived affordance idea] - [Brief explanation]
5. [Perceived affordance idea] - [Brief explanation]
[Optional additional ideas]
</perceived_affordances>

<signifiers>
1. [Signifier idea] - [Brief explanation]
2. [Signifier idea] - [Brief explanation]
3. [Signifier idea] - [Brief explanation]
4. [Signifier idea] - [Brief explanation]
5. [Signifier idea] - [Brief explanation]
[Optional additional ideas]
</signifiers>
</ideas>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 5 ideas in any required category.
- Explanations are missing for one or more ideas.
- No interaction analysis is provided before idea lists.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
