---
title: Empathy maps
category: User Research
tags:
  - user-research
  - empathy-map
  - personas
---
INPUTS
<provided_inputs>
- {{AUDIENCE}}
- {{TOPIC}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Empathy maps.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Build a detailed empathy map for `{{AUDIENCE}}` in relation to `{{TOPIC}}`.
- Include all eight categories:
- Thinks
- Feels
- Says
- Does
- Sees
- Hears
- Pains
- Goals
- For each category, provide 3-5 numbered insights that are specific, non-redundant, and behaviorally meaningful.
- Prioritize depth over surface-level statements, including motivations, fears, desires, social influences, and decision drivers where relevant.
- End with a concise summary of key takeaways and implications.

FORMAT
Return exactly this structure:

<empathy_map>
<thinks>
1. [Insight]
2. [Insight]
3. [Insight]
</thinks>

<feels>
1. [Insight]
2. [Insight]
3. [Insight]
</feels>

<says>
1. [Insight]
2. [Insight]
3. [Insight]
</says>

<does>
1. [Insight]
2. [Insight]
3. [Insight]
</does>

<sees>
1. [Insight]
2. [Insight]
3. [Insight]
</sees>

<hears>
1. [Insight]
2. [Insight]
3. [Insight]
</hears>

<pains>
1. [Insight]
2. [Insight]
3. [Insight]
</pains>

<goals>
1. [Insight]
2. [Insight]
3. [Insight]
</goals>

<summary>
[Brief key-takeaways and implications]
</summary>
</empathy_map>

FAILURE
- `<empathy_map>` wrapper or any required category/summary tag is missing or malformed.
- Any category has fewer than 3 insights.
- Insights are generic, repetitive across categories, or not tied to `{{AUDIENCE}}` and `{{TOPIC}}`.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
