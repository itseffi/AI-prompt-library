---
title: Product decision analysis from anthropological research insights
category: User Research
tags:
  - research
  - anthropology
  - product-strategy
  - user-personas
---
INPUTS
<provided_inputs>
- `{{ROLE}}`: Professional role perspective to combine with anthropological analysis.
- `{{USER_PERSONA}}`: The studied user group/persona.
- `{{TOPIC}}`: Product decision or topic to evaluate.
</provided_inputs>

GOAL
Evaluate a product decision through an anthropological lens grounded in deep understanding of a specific user group while maintaining objective analysis.
Success metric:
- Analysis covers all seven required dimensions of user-group fit and decision viability.
- Findings are specific, behavior-grounded, and actionable for product decisions.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs; if details are missing, state assumptions explicitly.
- Maintain third-person, objective analysis while reflecting deep empathy for the user group.
- Address all required dimensions:
1. Initial reactions
2. Relevance to daily life/goals/challenges
3. Adoption potential
4. Barriers
5. Opportunities
6. Modifications
7. Communication approach
- Ground claims in plausible observed behavior patterns, routines, motivations, and constraints of `{{USER_PERSONA}}`.
- Avoid generic advice; recommendations must tie directly to persona realities and `{{TOPIC}}`.
- Do not output scratchpad or hidden reasoning.

FORMAT
Return exactly this structure:

<analysis>
1. Initial Reactions: [Your insights here]
2. Relevance: [Your insights here]
3. Adoption Potential: [Your insights here]
4. Barriers: [Your insights here]
5. Opportunities: [Your insights here]
6. Modifications: [Your insights here]
7. Communication: [Your insights here]
</analysis>

FAILURE
- Output is not in the required `<analysis>` schema with all seven numbered sections.
- Any required dimension is missing, merged incorrectly, or materially incomplete.
- Claims are generic and not grounded in `{{USER_PERSONA}}` behaviors/motivations or `{{TOPIC}}` context.
- Analysis becomes purely subjective advocacy instead of objective, evidence-oriented framing.
- Assumptions are required but not explicitly stated.
