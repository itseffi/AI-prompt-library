---
title: App aha moment identification from user data and app description
category: User Research
tags:
  - user-research
  - analytics
  - activation
---
INPUTS
<provided_inputs>
- {{APP_DESCRIPTION}}
- {{USER_DATA}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: App aha moment identification from user data and app description.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{APP_DESCRIPTION}}` and `{{USER_DATA}}` to identify potential app "aha moment" conditions.
- Perform:
- Qualitative analysis to surface 3-5 likely activation actions/conditions and why they matter.
- Quantitative analysis of retained vs churned behavior, including strongest predictor metrics.
- Session/timing-sequence analysis when session-level data is available.
- Synthesize findings into top "aha moment" conditions and supporting evidence.
- For each potential condition, provide comparative engagement metrics where possible:
- `% users who performed condition and were retained`
- `% users who did not perform condition and were not retained`
- If required data is unavailable, state that explicitly and provide best-supported directional inference.

FORMAT
Return exactly this structure:

<analysis>
1. Qualitative Insights:
   [List your qualitative findings here]

2. Quantitative Insights:
   [List your quantitative findings here]

3. Potential "Aha Moment" Conditions:
   [List the top 3-5 conditions you've identified]

4. Supporting Metrics:
   [Provide relevant metrics for each condition]

5. Recommendations:
   [Offer 2-3 actionable recommendations to improve user activation based on your analysis]
</analysis>

FAILURE
- `<analysis>` schema is missing, malformed, or materially incomplete.
- Potential aha conditions are not 3-5 or are not tied to both qualitative and quantitative evidence.
- Supporting metrics are missing, non-comparative, or not derived from provided data.
- Session/timing insights are omitted when session data exists, or fabricated when it does not.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
