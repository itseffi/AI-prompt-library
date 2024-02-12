---
title: "Creative solution generation from De Bono's lateral thinking methods"
category: "Ideation & Creativity"
tags:
  - ideation
  - creativity
  - lateral-thinking
  - de-bono
  - problem-solving
  - product-management
---
INPUTS
<provided_inputs>
- {{PROBLEM}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Creative solution generation from De Bono's lateral thinking methods".
Success metric:
- Produces exactly 20 lateral provocations (`PO`) tied to the problem statement.
- Each provocation is converted into at least one plausible new option through a named De Bono movement approach.
- Provocations and options show clear variety (reversal, exaggeration, distortion, random connection).
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PROBLEM}}`; if context is incomplete, state assumptions explicitly.
- Generate exactly 20 provocations; each must begin with `PO:`.
- Ensure coverage across provocation types:
  - reversal,
  - exaggeration,
  - distortion,
  - random connection.
- For each provocation, apply at least one movement approach:
  - Abandon, Ideal case, Reversal, Exaggeration, Fortuity, or Falsification.
- For each provocation + approach, produce at least one concrete new option tied back to the original problem.
- Keep options specific enough to be testable/explorable (not generic slogans).

FORMAT
Return exactly this structure:

<creative_reframing>
<provocation_1>
PO: [Your provocation statement]  
Approach: [Approach used]  
New option: [Resulting idea or solution]
</provocation_1>

<provocation_2>
PO: [Your provocation statement]  
Approach: [Approach used]  
New option: [Resulting idea or solution]
</provocation_2>

[Continue for all 20 provocations]
</creative_reframing>

FAILURE
- Root tag `<creative_reframing>` is missing, malformed, or incomplete.
- Number of provocation blocks is not exactly 20.
- One or more provocations do not start with `PO:`.
- Any provocation block is missing `Approach` or `New option`.
- Provocations lack variety across the required provocation types.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
