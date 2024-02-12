---
title: Industry trend strategy
category: Product Strategy
tags:
  - strategy
  - competitive-analysis
  - positioning
  - decision-making
---
INPUTS
<provided_inputs>
- {{INDUSTRY}}
- {{TREND}}
- {{COMPANY}}
- {{GOAL}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Industry trend strategy.
Success metric:
- Produces a grounded industry + trend analysis tied to company strengths and goal.
- Proposes at least three distinct strategies with actionable steps.
- Summarizes how strategies leverage strengths to achieve the goal.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{INDUSTRY}}`, `{{TREND}}`, `{{COMPANY}}`, and `{{GOAL}}`; if critical data is missing, state assumptions explicitly.
- Provide a concise industry + trend analysis and a focused company strengths assessment.
- Propose at least 3 distinct strategies aligned to strengths and goal.
- Each strategy must include name, description, alignment, contribution to goal, challenges, and action steps.
- Keep recommendations specific and actionable, not generic.

FORMAT
Return exactly this structure:

<analysis>
[Industry + trend analysis and company strength assessment]
</analysis>

<strategies>
1. [Strategy name]
   - Description: [What it is]
   - Alignment: [Company strengths leveraged]
   - Contribution to goal: [How it advances the goal]
   - Challenges: [Risks/obstacles]
   - Action steps: [Concrete steps]
2. [Strategy name]
   - Description: ...
   - Alignment: ...
   - Contribution to goal: ...
   - Challenges: ...
   - Action steps: ...
3. [Strategy name]
   - Description: ...
   - Alignment: ...
   - Contribution to goal: ...
   - Challenges: ...
   - Action steps: ...
[Optional additional strategies]
</strategies>

<conclusion>
[Summary emphasizing how strategies leverage strengths to capitalize on the trend and achieve the goal]
</conclusion>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 3 strategies are provided.
- Strategies lack alignment to company strengths or contribution to goal.
- Action steps are missing or not actionable.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
