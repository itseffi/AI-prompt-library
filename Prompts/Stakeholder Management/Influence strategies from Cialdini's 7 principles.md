---
title: Influence strategies from Cialdini's 7 principles
category: Stakeholder Management
tags:
  - influence
  - cialdini
  - stakeholder-management
---
INPUTS
<provided_inputs>
- {{INFLUENCE_TARGET}}
- {{INFLUENCE_GOAL}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Influence strategies from Cialdini's 7 principles.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Generate influence ideas tailored to `{{INFLUENCE_TARGET}}` and `{{INFLUENCE_GOAL}}`.
- Provide at least one specific, actionable, ethical idea for each Cialdini principle:
- Reciprocity
- Liking
- Unity
- Authority
- Social Proof
- Consistency
- Scarcity
- For each idea, include a clear strategy and rationale tied to the target context and goal.
- Use professional, non-manipulative tactics that create value for both sides.

FORMAT
Return exactly this structure:

<influence_ideas>
<idea>
<principle>Name of the principle</principle>
<strategy>Detailed description of the strategy or tactic</strategy>
<rationale>Explanation of why this idea would be effective for the given target and goal</rationale>
</idea>
(Repeat this structure for each of the seven principles)
</influence_ideas>

FAILURE
- `<influence_ideas>` schema is missing, malformed, or materially incomplete.
- Not all seven principles are covered, or principles are duplicated while another is missing.
- Strategies are generic, unethical/manipulative, or not tied to the target and goal.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
