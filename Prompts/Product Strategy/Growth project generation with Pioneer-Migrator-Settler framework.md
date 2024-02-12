---
title: Growth project generation with Pioneer-Migrator-Settler framework
category: Product Strategy
tags:
  - strategy
  - growth
  - blue-ocean
  - innovation
  - portfolio
---
INPUTS
<provided_inputs>
- {{COMPANY}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Growth project generation with Pioneer-Migrator-Settler framework.
Success metric:
- Produces 12 distinct growth projects categorized into Pioneer/Migrator/Settler.
- Ensures balanced portfolio logic and a brief plan to drive growth.
- Keeps ideas concrete, differentiated, and aligned to the company context.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{COMPANY}}`; if details are missing, state assumptions explicitly.
- Generate exactly 12 distinct growth projects:
  - 3 creative,
  - 3 weird,
  - 3 compelling,
  - 3 novel and unexpected.
- Each idea must be tagged as one of: Pioneer, Migrator, Settler.
- Keep ideas concrete and specific to the company’s context.
- Provide a brief analysis of portfolio balance and strategic impact.
- Provide a short growth plan for how to build new market space and profitable growth.

FORMAT
Return exactly this structure:

<growth_projects>
<creative_ideas>
1. [Idea 1] - [Category]
2. [Idea 2] - [Category]
3. [Idea 3] - [Category]
</creative_ideas>

<weird_ideas>
1. [Idea 1] - [Category]
2. [Idea 2] - [Category]
3. [Idea 3] - [Category]
</weird_ideas>

<compelling_ideas>
1. [Idea 1] - [Category]
2. [Idea 2] - [Category]
3. [Idea 3] - [Category]
</compelling_ideas>

<novel_ideas>
1. [Idea 1] - [Category]
2. [Idea 2] - [Category]
3. [Idea 3] - [Category]
</novel_ideas>
</growth_projects>

<analysis>
[Brief analysis of mix and impact, with portfolio balance insights]
</analysis>

<growth_plan>
[Brief plan for creating new market space and profitable growth]
</growth_plan>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer or more than 12 ideas are provided.
- Any idea is missing a Pioneer/Migrator/Settler category.
- Ideas are generic or not grounded in the company context.
- Analysis or growth plan is missing or superficial.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
