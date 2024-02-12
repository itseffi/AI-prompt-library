---
title: Trade-off analysis from feature priority and effort data
category: Stakeholder Management
tags:
  - prioritization
  - tradeoffs
  - feature-evaluation
---
INPUTS
<provided_inputs>
- {{STAKEHOLDER_REQUEST}}
- {{FEATURE_PRIORITY}}
- {{FEATURE_EFFORT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Trade-off analysis from feature priority and effort data.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{STAKEHOLDER_REQUEST}}` using `{{FEATURE_PRIORITY}}` and `{{FEATURE_EFFORT}}`.
- Identify key benefits, drawbacks/opportunity costs, and lower-effort alternatives addressing similar needs.
- Build a 2x2 priority-effort matrix with quadrants:
- High Priority / Low Effort
- High Priority / High Effort
- Low Priority / Low Effort
- Low Priority / High Effort
- Place the proposed feature in the correct quadrant and include 2-3 comparator features/initiatives across other quadrants.
- Provide concise explanation for each matrix item (benefits, drawbacks, and placement rationale).
- Recommend whether to pursue, defer, or reject, with concrete next steps and alternatives.

FORMAT
Return exactly this structure:

<trade_off_analysis>
<matrix>
[Insert your 2x2 matrix here, using ASCII art or a simple text representation]
</matrix>

<explanations>
[Provide brief explanations for each item in the matrix]
</explanations>

<recommendation>
[Offer your recommendation and next steps]
</recommendation>
</trade_off_analysis>

FAILURE
- Any required section in `<trade_off_analysis>` is missing or materially incomplete.
- Matrix is missing the proposed feature or lacks 2-3 comparator items.
- Explanations do not justify quadrant placement with benefits/drawbacks.
- Recommendation is generic or does not provide clear next steps.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
