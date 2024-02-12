---
title: Feature impact models from KPIs and assumptions
category: Business Analysis
tags:
  - pm
  - business-analysis
  - financial-modeling
  - kpi-impact
---
INPUTS
<provided_inputs>
- {{FEATURE_INFO}}
- {{KPIS_TO_ESTIMATE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Feature impact models from KPIs and assumptions.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Follow these task requirements:
<task_requirements>
- Build a procedural task list that covers:
  - key assumptions,
  - baseline metric calculations,
  - per-KPI impact estimation,
  - sensitivity analysis.
- Execute the tasks and show calculations step by step using explicit formulas/equations.
- For each KPI, provide:
  - point estimate,
  - assumptions and calculations used,
  - brief explanation of feature-to-KPI impact mechanism.
- If information is missing, state what is missing, add a reasonable assumption, label it clearly, and proceed.
- Prioritize transparent math and reasoning over spreadsheet-like verbosity.
- Keep conclusions focused on executive decision-making (investment impact, major drivers, key risks).
</task_requirements>

FORMAT
Return exactly this structure:

<impact_size_model>
<procedural_tasks>
[List the procedural tasks used to build the model]
</procedural_tasks>

<calculations_and_assumptions>
[Step-by-step calculations, formulas, assumptions, and point estimates for each KPI]
</calculations_and_assumptions>

<summary>
[Feature overview, KPI estimate table/list, key assumptions, sensitivity-analysis takeaways, and executive conclusions]
</summary>
</impact_size_model>

FAILURE
- Output misses required sections, steps, or reasoning required by `<task_requirements>`.
- Required format/schema is missing, malformed, or incomplete.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
