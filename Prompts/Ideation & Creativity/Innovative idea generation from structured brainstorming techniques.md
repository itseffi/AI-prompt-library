---
title: "Innovative idea generation from structured brainstorming techniques"
category: "Ideation & Creativity"
tags:
  - brainstorming
  - structured-ideation
  - creativity
  - product-discovery
  - problem-solving
---
INPUTS
<provided_inputs>
- {{TOPIC}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Innovative idea generation from structured brainstorming techniques".
Success metric:
- Produces a structured ideation session using free association, mind mapping, SCAMPER, and bias checks.
- Generates non-obvious, high-potential ideas grounded in the topic.
- Outputs clear top ideas with rationale and a concise synthesis.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{TOPIC}}`; if scope is unclear, state assumptions explicitly.
- Run a complete structured ideation flow:
  - free association (4-6 rounds),
  - mind map (3-4 levels),
  - SCAMPER exploration (2-3 rounds across shortlisted branches),
  - bias check,
  - top-idea selection and rationale.
- Avoid clichéd or overhyped ideas; prioritize specificity and novelty.
- Ensure top ideas are distinct from one another and clearly connected to generated branches.
- Keep outputs practical enough to be explored/prototyped next.

FORMAT
Return exactly this structure:

<ideation_session>
<freeassociation>
[4-6 rounds of free associations tied to `{{TOPIC}}`]
</freeassociation>

<mindmap>
[Mind map with 3-4 branching levels derived from free associations]
</mindmap>

<shortlisted_branches>
1. [Branch]
2. [Branch]
3. [Branch]
</shortlisted_branches>

<scamper>
[2-3 rounds applying SCAMPER prompts to shortlisted branches]
</scamper>

<biascheck>
- Anchoring check: [Findings/adjustment]
- Status quo check: [Findings/adjustment]
- Groupthink check: [Findings/adjustment]
</biascheck>

<top_ideas>
1. [Idea 1]
2. [Idea 2]
3. [Idea 3]
</top_ideas>

<rationale>
1. [Why idea 1 is powerful and non-obvious]
2. [Why idea 2 is powerful and non-obvious]
3. [Why idea 3 is powerful and non-obvious]
</rationale>
</ideation_session>

<summary>
1. [Idea 1]: [Rationale]
2. [Idea 2]: [Rationale]
3. [Idea 3]: [Rationale]
</summary>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- `freeassociation` has fewer than 4 rounds or more than 6 rounds.
- `mindmap` does not show 3-4 levels of branching.
- `scamper` does not include at least 2 rounds.
- `top_ideas` does not contain exactly 3 distinct ideas.
- Rationales are generic and do not explain non-obvious value.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
