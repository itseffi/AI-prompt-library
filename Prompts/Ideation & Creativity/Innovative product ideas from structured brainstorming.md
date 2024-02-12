---
title: "Innovative product ideas from structured brainstorming"
category: "Ideation & Creativity"
tags:
  - brainstorming
  - product-ideas
  - structured-ideation
  - creativity
  - product-management
---
INPUTS
<provided_inputs>
- {{TOPIC}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Innovative product ideas from structured brainstorming".
Success metric:
- Produces a complete structured brainstorming session from divergence to convergence.
- Generates non-obvious product ideas grounded in the topic and validated via bias checks.
- Returns exactly 3 top ideas with clear innovation rationale in abstract terms.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{TOPIC}}`; if scope is unclear, state assumptions explicitly.
- Run all stages: free association, mind map, SCAMPER expansion, bias check, top-idea selection, summary.
- Avoid banal, overhyped, or clichéd outputs.
- Top ideas must be described abstractly; do not use specific tech buzzwords such as `AI`, `blockchain`, or `VR`.
- Ensure ideas are distinct and traceable to earlier brainstorming artifacts.

FORMAT
Return exactly this structure:

<brainstorming_session>

<free_association>
1. [Word or phrase]
2. [Word or phrase]
...
[Total 8-10 items]
</free_association>

<mind_map>
[Topic]
- [Main branch 1]
  - [Sub-branch 1a]
  - [Sub-branch 1b]
- [Main branch 2]
  - [Sub-branch 2a]
  - [Sub-branch 2b]
- [Main branch 3]
  - [Sub-branch 3a]
  - [Sub-branch 3b]
[At least 3 main branches; each with 2-3 sub-branches]
</mind_map>

<scamper>
- Branch: [Name]
  - Technique 1: [SCAMPER letter + method]
    - Application: [How applied]
    - New ideas:
      - [Idea]
  - Technique 2: [SCAMPER letter + method]
    - Application: [How applied]
    - New ideas:
      - [Idea]
[Repeat for 3 branches]
</scamper>

<bias_check>
- Bias: [Name]
  - Evidence in ideas: [How it appears]
  - Countermeasure: [Concrete action]
[At least 1 bias]
</bias_check>

<top_ideas>
1. [Idea title]
   - Description (2-3 sentences): [Abstract description]
   - Why innovative/non-obvious: [Rationale]
   - Topic fit (abstract): [How it addresses topic]
2. [Idea title]
   - Description (2-3 sentences): [Abstract description]
   - Why innovative/non-obvious: [Rationale]
   - Topic fit (abstract): [How it addresses topic]
3. [Idea title]
   - Description (2-3 sentences): [Abstract description]
   - Why innovative/non-obvious: [Rationale]
   - Topic fit (abstract): [How it addresses topic]
</top_ideas>

<summary>
[Brief recap of process and why final ideas are stronger after SCAMPER and bias checks]
</summary>

</brainstorming_session>

FAILURE
- Root tag `<brainstorming_session>` or any required sub-tag is missing, malformed, or incomplete.
- `free_association` has fewer than 8 or more than 10 items.
- `mind_map` has fewer than 3 main branches or insufficient sub-branches.
- `scamper` does not cover 3 branches with 2 techniques each.
- `top_ideas` does not contain exactly 3 ideas.
- Top ideas include banned specific-technology terms (`AI`, `blockchain`, `VR`).
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
