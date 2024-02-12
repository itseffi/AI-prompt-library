---
title: App design from project requirements
category: Design & Prototyping
tags:
  - app-design
  - ux
  - design-system
  - wireframing
---
INPUTS
<provided_inputs>
- {{PROJECT_DESCRIPTION}}
- {{TARGET_AUDIENCE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: App design from project requirements.
Success metric:
- Defines one clear core feature aligned to user needs and project goals.
- Provides a functional grayscale interface sketch focused on essential flow.
- Produces a minimal, consistent design system within stated constraints.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PROJECT_DESCRIPTION}}` and `{{TARGET_AUDIENCE}}`; if details are missing, state assumptions explicitly.
- Identify exactly one core feature (the single highest-value user task).
- Keep interface sketch grayscale/function-first and limited to essential elements for the core feature.
- Design system must remain lightweight:
  - Font sizes: 3-4 sizes total.
  - Colors: 1 primary + up to 2-3 secondary colors.
  - Spacing: one consistent scale.
  - Button styles: 1-2 styles.
- Keep choices practical, internally consistent, and audience-appropriate.

FORMAT
Return exactly this structure:

<kickoff_plan>
<core_feature>
[Insert your defined core feature here]
</core_feature>

<interface_sketch>
[Describe your grayscale interface sketch here. Be specific about layout and essential elements.]
</interface_sketch>

<design_system>
<font_sizes>
[List your chosen font sizes]
</font_sizes>

<colors>
[List your chosen colors]
</colors>

<spacing_values>
[Describe your spacing scale]
</spacing_values>

<button_styles>
[Describe your button style(s)]
</button_styles>
</design_system>
</kickoff_plan>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- More than one core feature is proposed.
- `interface_sketch` emphasizes visual styling over functional layout.
- `font_sizes` has fewer than 3 or more than 4 sizes.
- `colors` exceeds 1 primary + 2-3 secondary colors.
- `button_styles` has fewer than 1 or more than 2 styles.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
