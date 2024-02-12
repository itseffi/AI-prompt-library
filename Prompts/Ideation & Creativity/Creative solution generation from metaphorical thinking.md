---
title: "Creative solution generation from metaphorical thinking"
category: "Ideation & Creativity"
tags:
  - ideation
  - creativity
  - metaphor
  - problem-solving
  - perspective-shifting
---
INPUTS
<provided_inputs>
- {{ISSUE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Creative solution generation from metaphorical thinking".
Success metric:
- Produces at least 3 issue metaphors with clear relevance to the issue.
- Generates 20 distinct random activities and maps each to at least one meaningful similarity.
- Selects one best metaphor from the activity list with a compelling rationale.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{ISSUE}}`; if context is incomplete, state assumptions explicitly.
- Provide at least 3 metaphors directly representing the issue.
- Generate exactly 20 random activities and avoid these examples: building a house, raising a child, cooking a meal.
- For each activity, provide at least one explicit similarity to the issue.
- Choose one best metaphor from the activity list (not from outside the list) and explain insight gained.
- Keep connections concrete enough to inspire actionable reframing (not generic one-liners).

FORMAT
Return exactly this structure:

<output>
<issue_metaphors>
1. [Metaphor] - [How it relates to the issue]
2. [Metaphor] - [How it relates to the issue]
3. [Metaphor] - [How it relates to the issue]
[Optional additional metaphors]
</issue_metaphors>

<random_activities>
1. [Activity]
2. [Activity]
...
20. [Activity]
</random_activities>

<activity_similarities>
1. [Activity 1] - [Similarity to issue]
2. [Activity 2] - [Similarity to issue]
...
20. [Activity 20] - [Similarity to issue]
</activity_similarities>

<best_metaphor>
[State the activity you chose as the best metaphor and explain why]
</best_metaphor>
</output>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 3 issue metaphors are provided.
- Random activities count is not exactly 20.
- Any activity lacks a corresponding similarity mapping.
- Best metaphor is not selected from the listed random activities.
- Disallowed example activities are reused.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
