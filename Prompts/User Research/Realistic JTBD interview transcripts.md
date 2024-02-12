---
title: Realistic JTBD interview transcripts
category: User Research
tags:
  - user-research
  - jtbd
  - interviews
---
INPUTS
<provided_inputs>
- `{{PRODUCT_TYPE}}`: Product category to explore.
- `{{TARGET_AUDIENCE}}`: Core audience profile for the interview.
- `{{NUM_PARTICIPANTS}}`: Number of participants to include in the transcript.
</provided_inputs>

GOAL
Generate a realistic multi-participant JTBD interview transcript that surfaces the four forces of progress (push, pull, anxiety, habit) through natural conversation.
Success metric:
- Transcript is realistic, exploratory, and participant-driven.
- Conversation captures current behaviors, pain points, desired outcomes, switching concerns, and habits.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs; if details are missing, state assumptions briefly in the handover.
- Role-play both Product Designer and participants in a realistic dialogue.
- Product Designer behavior must be:
- Open-ended questioning.
- Follow-up on ambiguity and interesting signals.
- Encouraging elaboration.
- Non-leading and solution-neutral.
- Curious and empathetic tone.
- Cover these conversation phases naturally:
1. Introduction and warm-up.
2. Current solutions and pain points.
3. Desired outcomes and aspirations.
4. Concerns and hesitations about change.
5. Existing routines and habitual behaviors.
- Ensure all participants contribute meaningfully.
- Reveal the four JTBD forces implicitly through content, without naming them explicitly.

FORMAT
Return exactly this structure:

<transcript>
Product Designer: [Introduction and first question]

Participant 1: [Response]

Product Designer: [Follow-up question]

Participant 2: [Response]

[Continue until all participants contribute and the conversation feels complete.]
</transcript>

<handover>
This concludes the interview transcript. What specific aspects of the conversation would you like me to elaborate on or analyze further?
</handover>

FAILURE
- Output is missing either `<transcript>` or `<handover>`.
- Transcript does not include the Product Designer plus the requested number of participants.
- Conversation is generic, shallow, or fails to cover required interview phases.
- Product Designer asks leading/solution-prescriptive questions.
- Four JTBD force signals are not inferable from the dialogue.
- Participants do not contribute meaningfully or are not differentiated.
- Assumptions are required but not explicitly noted in handover.
