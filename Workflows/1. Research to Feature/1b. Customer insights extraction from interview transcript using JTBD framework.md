---
title: Customer insights extraction from interview transcript using JTBD framework
category: User Research
tags:
  - user-research
  - interviews
  - jtbd
---
INPUTS
<provided_inputs>
- {{INTERVIEW_TRANSCRIPT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Customer insights extraction from interview transcript using JTBD framework.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{INTERVIEW_TRANSCRIPT}}` using JTBD forces:
- Pushes.
- Pulls.
- Habits.
- Anxieties.
- Extract force statements with required phrasing:
- Pushes and Habits as `When...` statements.
- Pulls as `So I can...` / `So I don't...` statements.
- Anxieties as concerns/questions.
- Synthesize decision dynamics including:
- Decision criteria.
- Trade-offs interviewee accepts.
- Functional, social, and emotional priorities.
- Ground all outputs in transcript evidence and state assumptions only when necessary.

FORMAT
Return exactly this structure:

<analysis>
<context>
[Briefly describe the interviewee's current situation, job, and challenges]
</context>

<pushes>
[List the identified "When..." statements for Pushes]
</pushes>

<pulls>
[List the identified "So I can..." or "So I don't..." statements for Pulls]
</pulls>

<habits>
[List the identified "When..." statements for Habits]
</habits>

<anxieties>
[List the identified questions or statements of concern for Anxieties]
</anxieties>

<insights>
[Provide a summary of your insights about the interviewee's decision-making process]
</insights>
</analysis>

FAILURE
- Any required section in `<analysis>` is missing or materially incomplete.
- JTBD force phrasing rules are not followed (`When...`, `So I can.../So I don't...`, anxiety concerns).
- Insights do not cover decision criteria, trade-offs, and functional/social/emotional drivers.
- Statements are generic or not grounded in transcript evidence.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
