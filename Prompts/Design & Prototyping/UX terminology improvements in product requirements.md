---
title: "UX terminology improvements in product requirements"
category: "Design & Prototyping"
tags:
  - ux
  - product-requirements
  - terminology
  - content-review
---
INPUTS
<provided_inputs>
- {{PRODUCT_MANAGER_REQUIREMENTS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "UX terminology improvements in product requirements".
Success metric:
- Identifies incorrect or imprecise UX terminology in the requirements, when present.
- Provides context-appropriate terminology corrections with clear rationale.
- Avoids unnecessary edits when wording is already accurate.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT_MANAGER_REQUIREMENTS}}`; if context is missing, state assumptions explicitly.
- Review terms in context; do not auto-replace words without justification.
- For each correction, quote the original wording exactly.
- Provide a correction only when it improves UX precision/clarity.
- If no corrections are needed, explicitly return the no-change statement in the required schema.

FORMAT
Return exactly this structure:

<analysis>
1. Original term: [Quote the original text]  
   Correction: [Provide the corrected term or phrase]  
   Explanation: [Briefly explain why this correction is necessary]

2. Original term: [Quote the original text]  
   Correction: [Provide the corrected term or phrase]  
   Explanation: [Briefly explain why this correction is necessary]

[Continue with additional corrections as needed]

[If no corrections are required, return exactly:
"No corrections needed. The requirements use appropriate UX terminology."]
</analysis>

FAILURE
- `<analysis>` section is missing or malformed.
- Corrections are provided without quoting original text.
- Explanations do not justify why the correction improves UX terminology precision.
- Output changes terminology that is already context-appropriate without rationale.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
