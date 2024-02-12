---
title: Product simplification via Via Negativa analysis
category: Business Analysis
tags:
  - pm
  - business-analysis
  - simplification
  - via-negativa
  - strategy
---
INPUTS
<provided_inputs>
- {{INPUT}}
</provided_inputs>

GOAL
Apply Via Negativa to simplify `INPUT` by removing non-essential elements while preserving core purpose and functional integrity.
Success metric:
- Clearly defines core purpose.
- Identifies non-essential elements with rationale, benefits of removal, and tradeoffs.
- Produces a simplified version that remains aligned to the core purpose.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required reasoning steps:
  1. Identify core purpose.
  2. Enumerate major elements/components.
  3. Test each element for necessity, value, replaceability, and complexity cost.
  4. Select removals/simplifications that preserve purpose.
  5. Evaluate downside risks of each removal.
- Keep recommendations concrete and grounded in provided input details.
- Prefer removal/simplification over additive fixes.
- Explicitly label assumptions when input details are ambiguous.

FORMAT
Return exactly this structure:

<via_negativa_analysis>
<core_purpose>
Briefly state the identified core purpose or main objective of the input.
</core_purpose>

<non_essential_elements>
List the elements you've identified as non-essential, explaining for each:
- Why it's considered non-essential
- How removing it could benefit the overall input
- Any potential drawbacks of its removal
</non_essential_elements>

<simplified_version>
Provide a simplified version of the input, focusing only on the essential elements that directly contribute to the core purpose.
</simplified_version>

<conclusion>
Summarize how the simplified version aligns better with the principles of Via Negativa and how it improves upon the original input in terms of clarity, efficiency, and focus.
</conclusion>
</via_negativa_analysis>

FAILURE
- Any required schema section is missing or malformed.
- Non-essential elements are listed without rationale, benefit, and drawback analysis.
- Simplified version changes core purpose or omits critical essentials.
- Claims are generic or not grounded in provided input.
- Assumptions are used but not explicitly stated.
