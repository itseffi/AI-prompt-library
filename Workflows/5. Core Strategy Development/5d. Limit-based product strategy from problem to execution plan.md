---
title: Limit-based product strategy from problem to execution plan
category: Product Strategy
tags:
  - product-strategy
  - roadmapping
  - long-term-thinking
  - structured-thinking
---
INPUTS
<provided_inputs>
- {{PROBLEM_STATEMENT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Limit-based product strategy from problem to execution plan.
Success metric:
- Applies the full Limit-Based Product Thinking framework end-to-end.
- Produces concrete milestones, levers, assumptions, and a phased execution plan.
- Keeps outputs grounded in the provided problem statement.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PROBLEM_STATEMENT}}`; if critical details are missing, state assumptions explicitly.
- Follow all 7 framework steps in order.
- Provide quantified convergence milestones at 10%, 25%, 50%, 75%, 90% with dates or triggers.
- Identify levers to accelerate convergence and explicitly name the top 1–2 highest impact moves.
- List critical assumptions with validation methods.
- Provide a 3-phase plan (Foundation, Acceleration, Optimization) with timelines and resource guidance.

FORMAT
Return exactly this structure:

<limit_based_analysis>
1. Growth Variable: [Your identified variable]

2. Limit State Description:
   [Your vivid description of the fully mature state]

3. Core Properties of the Limit:
   [List of key features and interactions]

4. Convergence Estimate:
   [Growth curve and milestones]

5. Acceleration Strategies:
   [Prioritized list of levers to steepen the curve]

6. Critical Assumptions:
   [List of assumptions with validation methods]

7. Product Vision and Execution:
   Vision Statement: [One-sentence summary]  
   Roadmap: [Major milestones and timelines]  
   3-Phase Plan: [Brief outline of each phase]  
   Resource Allocation: [Key recommendations]

</limit_based_analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Convergence milestones are missing required percentages or triggers/dates.
- Acceleration strategies lack prioritized top 1–2 levers.
- Assumptions lack validation methods.
- 3-phase plan is missing or not sequenced.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
