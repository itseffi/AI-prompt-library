---
title: "Decision reversibility classification from first principles"
category: "Decision Making"
tags:
  - pm
  - decision-making
  - reversibility
  - first-principles
  - frameworks
---
INPUTS
<provided_inputs>
- {{SITUATION}}
- {{DECISION}}
</provided_inputs>

GOAL
Classify a decision’s reversibility from first principles as `Hat`, `Haircut`, or `Tattoo`, with explicit reasoning.
Success metric:
- Evaluates immediate and long-term consequences.
- Assesses reversal cost/time/resources and permanence.
- Produces a defensible classification with confidence and rationale.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required dimensions:
  1. Immediate consequences.
  2. Long-term effects on stakeholders/environment.
  3. Reversal effort/time/resource requirements.
  4. Permanent or hard-to-undo changes.
- Apply category definitions strictly:
  - `Hat`: easily reversible; minimal lasting consequences.
  - `Haircut`: reversible with meaningful but manageable cost/friction.
  - `Tattoo`: largely irreversible or long-lasting structural impact.
- Consider multiple plausible outcomes; avoid single-path reasoning.
- Keep analysis neutral and grounded in `SITUATION` and `DECISION`.
- Explicitly label assumptions where context is incomplete.

FORMAT
Return exactly this structure:

<analysis>
<immediate_consequences>[Assessment]</immediate_consequences>
<long_term_effects>[Assessment]</long_term_effects>
<reversal_cost_and_feasibility>[Assessment of effort/time/resources]</reversal_cost_and_feasibility>
<permanence_factors>[What becomes hard or impossible to undo]</permanence_factors>
<synthesis>[How the above dimensions combine into a final judgment]</synthesis>
</analysis>

<categorization>
[Hat | Haircut | Tattoo]
</categorization>
<confidence>
[High | Medium | Low] - [Brief reason]
</confidence>
<reversal_path>
[If reversible, concise path to reverse/mitigate; if tattoo, explain why reversal is impractical]
</reversal_path>

FAILURE
- Required schema sections are missing or malformed.
- Classification is provided without first-principles reasoning across required dimensions.
- Category choice contradicts stated evidence.
- Analysis is generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
