---
title: Decision-making with the GUT CHECK protocol
category: Decision Making
tags:
  - decision-making
  - self-reflection
  - frameworks
  - coaching
---
INPUTS
<provided_inputs>
- {{DECISION}}
</provided_inputs>

GOAL
Guide the user through the full GUT CHECK protocol for `DECISION`, then provide a grounded recommendation.
Success metric:
- Covers all 8 GUT CHECK stages with relevant reflective questions.
- Separates prompts/questions from interpretation clearly.
- Provides a summary and final recommendation consistent with the surfaced signals.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Cover all 8 protocol stages:
  1. Pause & Feel
  2. Identify Pressures
  3. Risk Assessment
  4. Competency Check
  5. Values Alignment
  6. Timing Check
  7. Red Flags
  8. Final Gut Check
- For each stage, provide concise reflection prompts tailored to `DECISION`.
- Keep tone supportive, neutral, and non-judgmental.
- If user responses are not available, mark insights as provisional and identify what responses are needed.
- Include the pressure mantra and key protocol reminders.
- Final recommendation must align with surfaced signals (not generic advice).

FORMAT
Return exactly this structure:

<gut_check_protocol>
<pause_and_feel>[Stage-specific prompts]</pause_and_feel>
<identify_pressures>[Stage-specific prompts]</identify_pressures>
<risk_assessment>[Stage-specific prompts]</risk_assessment>
<competency_check>[Stage-specific prompts]</competency_check>
<values_alignment>[Stage-specific prompts]</values_alignment>
<timing_check>[Stage-specific prompts]</timing_check>
<red_flags>[Stage-specific prompts and pause rule]</red_flags>
<final_gut_check>[Stage-specific prompts]</final_gut_check>
<mantra>"This is now. Whatever comes, I can handle it. Next step forward."</mantra>
<protocol_reminders>[Key points about gut/hidden costs/alternate paths/well-being]</protocol_reminders>
</gut_check_protocol>

<summary>
[Summary of user responses if provided; otherwise a provisional synthesis and missing-response checklist]
</summary>

<recommendation>
[Provide a final recommendation based on the user's responses, explaining the reasoning behind it]
</recommendation>

FAILURE
- Missing any required stage in `<gut_check_protocol>`, `<summary>`, or `<recommendation>`.
- Recommendation is generic or not supported by protocol signals.
- Tone is judgmental, coercive, or dismissive.
- Missing provisional labeling when user responses are unavailable.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
