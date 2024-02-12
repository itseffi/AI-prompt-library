---
title: Business flywheel from company successes and failures
category: Product Strategy
tags:
  - strategy
  - flywheel
  - hedgehog-concept
  - retrospectives
  - business-model
---
INPUTS
<provided_inputs>
- {{COMPANY_INFO}}
- {{SUCCESSES}}
- {{DISAPPOINTMENTS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Business flywheel from company successes and failures.
Success metric:
- Produces a 4–6 component flywheel grounded in successes and disappointments.
- Explains the causal loop and how it reinforces outcomes.
- Connects the flywheel to Hedgehog Concept alignment.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{COMPANY_INFO}}`, `{{SUCCESSES}}`, and `{{DISAPPOINTMENTS}}`; if information is missing, state assumptions explicitly.
- Identify 4–6 flywheel components only; consolidate if more.
- Describe the causal loop explicitly (component -> component).
- Validate the flywheel against successes and disappointments (explain fit and gaps).
- Map the flywheel to the Hedgehog Concept circles.
- Keep outputs specific and evidence-grounded; avoid generic platitudes.

FORMAT
Return exactly this structure:

<flywheel_analysis>
<components>
List the 4–6 key components you've identified.
</components>

<flywheel_sketch>
Describe the flywheel, explaining how each component leads to the next in a self-reinforcing loop.
</flywheel_sketch>

<success_alignment>
Explain how the flywheel aligns with and explains the company's successes.
</success_alignment>

<disappointment_insights>
Describe how the flywheel provides insights into the company's disappointments or failures.
</disappointment_insights>

<hedgehog_alignment>
Discuss how the flywheel aligns with the three circles of the Hedgehog Concept.
</hedgehog_alignment>
</flywheel_analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Number of flywheel components is outside 4–6.
- Flywheel sketch does not show a clear causal loop.
- Alignment sections are generic or not tied to provided inputs.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
