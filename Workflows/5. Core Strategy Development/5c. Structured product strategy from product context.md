---
title: Structured product strategy from product context
category: Product Strategy
tags:
  - product-strategy
  - roadmapping
  - product-management
  - structured-thinking
  - product-vision
---
INPUTS
<provided_inputs>
- {{PRODUCT_CONTEXT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Structured product strategy from product context.
Success metric:
- Produces a complete strategy across objective, users, superpowers, vision, pillars, impact, and roadmap.
- Keeps each section grounded in the provided product context.
- Provides concrete, coherent outputs that build on each other.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT_CONTEXT}}`; if context is missing, state assumptions explicitly.
- Provide all 7 sections in the required format.
- Objective: 1–2 sentences, ambitious but achievable.
- Users: 1–2 groups; each with 3–4 needs.
- Superpowers: 3–4 unique advantages.
- Vision: 2–3 paragraphs.
- Pillars: 2–4 themes with brief descriptions.
- Impact: causal mechanism or back-of-envelope logic.
- Roadmap: 3–10 items per pillar (no prioritization).

FORMAT
Return exactly this structure:

<product_strategy>

<objective>

[Your objective here]

</objective>

<users>

[User group descriptions and bullet points here]

</users>

<superpowers>

[List of superpowers here]

</superpowers>

<vision>

[Your vision paragraphs here]

</vision>

<pillars>

[List of pillars with titles and descriptions here]

</pillars>

<impact>

[Impact description here]

</impact>

<roadmap>

[Roadmap items for each pillar here]

</roadmap>

</product_strategy>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Counts are outside required ranges (users, superpowers, pillars, roadmap items).
- Impact does not explain mechanism or is generic.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
