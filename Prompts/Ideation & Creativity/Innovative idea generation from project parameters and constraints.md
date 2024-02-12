---
title: "Innovative idea generation from project parameters and constraints"
category: "Ideation & Creativity"
tags:
  - creativity
  - idea-generation
  - constraints
  - product-management
  - osborn-checklist
---
INPUTS
<provided_inputs>
- {{PROJECT_TYPE}}
- {{GOALS}}
- {{BUDGET}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Innovative idea generation from project parameters and constraints".
Success metric:
- Produces concrete, non-generic ideas that fit project type, goals, and budget.
- Uses structured creativity analysis (including Osborn checklist) to move beyond obvious solutions.
- Final ideas are immediately actionable with clear execution steps.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PROJECT_TYPE}}`, `{{GOALS}}`, and `{{BUDGET}}`; if details are missing, state assumptions explicitly.
- Provide exactly 5 banal ideas to avoid and explain why each is weak.
- Define problem context including timeframe, target audience, and situation.
- Break down problem into objective, constraints, measurable success criteria, challenges, and deeper considerations.
- Analyze each chunk with explicit link to goals and budget feasibility.
- Include both creator and consumer perspectives.
- Apply Osborn checklist categories with project-relevant outputs:
  - other uses, adaptations, modifications, magnification, minification, substitutions, rearrangements, reversals, combinations.
- Final ideas must be actionable for an individual, feasible under budget, and include step-by-step instructions plus application context.

FORMAT
Return exactly this structure:

<creativity_analysis>
<banal_ideas>
1. [Banal idea] - [Why to avoid]
2. [Banal idea] - [Why to avoid]
3. [Banal idea] - [Why to avoid]
4. [Banal idea] - [Why to avoid]
5. [Banal idea] - [Why to avoid]
</banal_ideas>

<problem_definition>
[Clearly define the problem or situation]
</problem_definition>

<problem_breakdown>
[Break down the problem into key aspects]
</problem_breakdown>

<chunk_analysis>
[Provide in-depth analysis of each problem chunk]
</chunk_analysis>

<perspectives>
[Describe creator and consumer perspectives]
</perspectives>

<osborn_checklist>
- Other uses: [Ideas]
- Adaptations: [Ideas]
- Modifications: [Ideas]
- Magnification: [Ideas]
- Minification: [Ideas]
- Substitutions: [Ideas]
- Rearrangements: [Ideas]
- Reversals: [Ideas]
- Combinations: [Ideas]
</osborn_checklist>

<final_ideas>
1. [Idea title]
   - Specific guidance: [What to do]
   - Steps: [Step-by-step]
   - Where/how to apply: [Context/channel/tool]
   - Budget fit: [How it stays within budget]
[Repeat for additional ideas]
</final_ideas>
</creativity_analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- `banal_ideas` does not contain exactly 5 items.
- One or more Osborn checklist categories are missing.
- Final ideas are not actionable step-by-step or are not aligned to budget/goals.
- Output is generic or repeats cliché ideas without meaningful differentiation.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
