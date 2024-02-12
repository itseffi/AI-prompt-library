---
title: "Product strategy review from draft documents"
category: "Product Strategy"
tags:
  - product-management
  - strategy
  - stakeholder-management
  - communication
---
INPUTS
<provided_inputs>
- {{DRAFT_DOCUMENT}}
- {{CONTEXT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Product strategy review from draft documents".
Success metric:
- Produces a high-signal review of strengths, gaps, and review risks in the draft.
- Provides concrete copy/structure improvements that can be directly used in the draft.
- Surfaces the top 3 discussion points likely to drive executive review decisions.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{DRAFT_DOCUMENT}}` and `{{CONTEXT}}`; if data is missing, state assumptions explicitly.
- Analyze strengths and gaps against:
  - punchline clarity,
  - front-loading of controversial elements,
  - memorable insight/stat,
  - customer pain articulation,
  - solution-to-pain alignment,
  - assumptions/trade-offs,
  - executive question readiness.
- In `<analysis>`, use a numbered list; each item is 2-3 sentences, with the first short sentence in bold.
- In `<improvements>`, provide up to 10 concrete copy/structure edits in the same style as the draft.
- Do not fabricate data or claims; explicitly call out missing data when needed.
- Output only the required tags and nothing outside them.

FORMAT
Return exactly this structure:

<analysis>
[Numbered list of strengths and gaps; first short sentence bold in each item]
</analysis>

<improvements>
[Numbered list (up to 10) of specific copy and structure improvements]
</improvements>

<discussion_points>
[Your list of top 3 discussion points]
</discussion_points>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- `<analysis>` items do not follow the required format (numbered, 2-3 sentences, bold first short sentence).
- `<improvements>` has more than 10 items or lacks concrete rewrites.
- `discussion_points` does not contain exactly 3 points.
- Output includes fabricated data not present in inputs.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
