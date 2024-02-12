---
title: Pyramid structure optimization from complex text
category: Presentation & Communication
tags:
  - writing
  - storytelling
  - presentations
  - structured-thinking
---
INPUTS
<provided_inputs>
- {{TEXT_TO_OPTIMIZE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Pyramid structure optimization from complex text.
Success metric:
- Produces a clear Minto-style pyramid with one key message and 2-3 supporting arguments.
- Uses only evidence/details traceable to the source text.
- Improves clarity and concision while preserving core meaning.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{TEXT_TO_OPTIMIZE}}`; if key context is missing, state assumptions explicitly.
- Identify exactly one key message.
- Provide 2-3 supporting arguments (no more than 3).
- Attach evidence/details for each argument using source-grounded points only.
- Lead with conclusion first, then grouped support (Minto Pyramid Principle).
- Keep wording concise and structured; avoid unnecessary prose.

FORMAT
Return exactly this structure:

<optimized_text>
Key Message: [Insert the main conclusion or recommendation]

Supporting Arguments:
1. [First main argument]
   - [Evidence or detail]
   - [Evidence or detail]

2. [Second main argument]
   - [Evidence or detail]
   - [Evidence or detail]

3. [Third main argument (if applicable)]
   - [Evidence or detail]
   - [Evidence or detail]
</optimized_text>

<explanation>
[Brief explanation of what was changed and why communication is clearer]
</explanation>

FAILURE
- `<optimized_text>` or `<explanation>` is missing, malformed, or incomplete.
- More than one key message is provided.
- Fewer than 2 or more than 3 supporting arguments are provided.
- Supporting evidence is generic or not traceable to the source text.
- Structure starts with details instead of the key message.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
