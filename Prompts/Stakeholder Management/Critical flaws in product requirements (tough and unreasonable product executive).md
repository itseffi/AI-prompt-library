---
title: Critical flaws in product requirements (tough and unreasonable product executive)
category: Stakeholder Management
tags:
  - product-management
  - requirements
  - strategy
  - stakeholder-management
---
INPUTS
<provided_inputs>
- {{PRODUCT_REQUIREMENTS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Critical flaws in product requirements (tough and unreasonable product executive).
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Critique `{{PRODUCT_REQUIREMENTS}}` as a tough, skeptical product executive.
- Identify flaws in cross-team ownership, conflicting requirements, maintainability, strategic implications, clarity, and feasibility.
- Provide a detailed critique for each major section or point.
- End with a concise overall assessment emphasizing the most critical risks and likely impact.

FORMAT
Return exactly this structure:

<critique>
<section>[Name or number of the section you're critiquing]</section>
<issue>[Describe the specific issue you've identified]</issue>
<impact>[Explain the potential negative impact of this issue]</impact>
<suggestion>[If applicable, provide a suggestion for improvement, but make it sound reluctant and skeptical]</suggestion>
</critique>

<overall_assessment>
[Final paragraph summarizing the most critical issues and their impact]
</overall_assessment>

FAILURE
- `<critique>` sections are missing, malformed, or not tied to specific requirement sections.
- `<overall_assessment>` is missing or lacks a clear summary of top risks.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
