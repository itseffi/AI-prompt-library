---
title: "Product design analysis from context and screenshots"
category: "Design & Prototyping"
tags:
  - pm
  - ux
  - design
  - critique
  - analysis
---
INPUTS
<provided_inputs>
- {{CONTEXT}}
- {{SCREENSHOTS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Product design analysis from context and screenshots".
Success metric:
- Identifies concrete design issues from provided context/screenshots.
- Recommends optimization opportunities tied to stated goals and metrics.
- Provides viable alternative approaches with clear tradeoffs.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{CONTEXT}}` and `{{SCREENSHOTS}}`; if details are missing, state assumptions explicitly.
- Ground every issue and recommendation in observable evidence from context/screenshots.
- Prioritize findings by likely impact on user outcomes and stated product goals/metrics.
- Keep recommendations actionable, testable, and specific (not generic UX advice).
- Include balanced tradeoffs when proposing alternatives.

FORMAT
Return exactly this structure:

<analysis>
<issues_and_limitations>
- [Issue 1] - [Evidence from context/screenshot] - [Why it is a limitation]
- [Issue 2] - [Evidence from context/screenshot] - [Why it is a limitation]
[Additional issues as needed]
</issues_and_limitations>

<optimization_opportunities>
- [Opportunity 1] - [Target goal/metric] - [Suggested change] - [Expected impact]
- [Opportunity 2] - [Target goal/metric] - [Suggested change] - [Expected impact]
[Additional opportunities as needed]
</optimization_opportunities>

<alternative_approaches>
- [Alternative 1] - [What changes] - [Pros] - [Cons]
- [Alternative 2] - [What changes] - [Pros] - [Cons]
[Additional alternatives as needed]
</alternative_approaches>

<pros_and_cons>
- Pros:
  - [Pro 1]
  - [Pro 2]
- Cons:
  - [Con 1]
  - [Con 2]
</pros_and_cons>
</analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Issues/recommendations are not traceable to provided context/screenshots.
- Optimization opportunities are not tied to product goals/metrics.
- Alternatives are listed without explicit pros/cons tradeoffs.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
