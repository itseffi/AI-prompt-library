---
title: Competitive analysis to winning positioning strategy
category: Product Strategy
tags:
  - positioning
  - competition
  - product-marketing
  - differentiation
---
INPUTS
<provided_inputs>
- {{COMPETITIVE_ANALYSIS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Competitive analysis to winning positioning strategy.
Success metric:
- Produces a data-backed positioning strategy grounded in competitive analysis.
- Identifies 3–5 clear differentiators with customer-relevant rationale.
- Outputs a concise, compelling value proposition and the reasoning behind it.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{COMPETITIVE_ANALYSIS}}`; if data is missing, state assumptions explicitly.
- Identify 3–5 differentiators grounded in the competitive analysis.
- For each differentiator, explain customer value and competitive significance.
- Define a clear target audience and market position based on evidence.
- Value proposition must answer “why choose us” without introducing unsupported claims.

FORMAT
Return exactly this structure:

<differentiators>
1. [Differentiator] - [Why it matters to customers] - [Evidence from analysis]
2. [Differentiator] - [Why it matters to customers] - [Evidence from analysis]
3. [Differentiator] - [Why it matters to customers] - [Evidence from analysis]
[Optional 4th/5th differentiator]
</differentiators>

<positioning_strategy>
[Target audience, market position, and how differentiators map to customer needs and gaps]
</positioning_strategy>

<unique_value_proposition>
[Concise statement answering why choose us]
</unique_value_proposition>

<rationale>
[Explain reasoning with explicit references to competitive analysis]
</rationale>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 3 or more than 5 differentiators are provided.
- Positioning or value proposition is not grounded in provided analysis.
- Rationale lacks evidence references.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
