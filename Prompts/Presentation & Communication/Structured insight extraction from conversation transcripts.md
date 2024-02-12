---
title: Structured insight extraction from conversation transcripts
category: Presentation & Communication
tags:
  - conversation-analysis
  - transcripts
  - insight-extraction
  - presentation
  - communication
---
INPUTS
<provided_inputs>
- {{CONVERSATION_TRANSCRIPT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Structured insight extraction from conversation transcripts.
Success metric:
- Produces a faithful, structured reconstruction of the conversation flow and outcomes.
- Identifies participants, branches, responsibilities, current status, and open items.
- Keeps all claims grounded in the transcript without adding assumptions.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{CONVERSATION_TRANSCRIPT}}`; do not infer roles or tasks not stated.
- Identify all participants and their roles (if roles are unclear, note `Unknown`).
- Summarize conversation flow and any branching points.
- Capture participant responsibilities and open items explicitly mentioned.
- Keep output strictly within the required tags; no scratchpad in final output.

FORMAT
Return exactly this structure:

<analysis>
<participants>
[List of participants and their roles]
</participants>

<conversation_flow>
[Summary of the conversation's progression]
</conversation_flow>

<conversation_branches>
[List of significant branches or shifts in the conversation]
</conversation_branches>

<participant_responsibilities>
[Summary of each participant's tasks or responsibilities]
</participant_responsibilities>

<current_status>
[Summary of where the conversation has landed]
</current_status>

<open_items>
[List of any open questions or tasks]
</open_items>
</analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Participants or responsibilities are inferred without transcript evidence.
- Open items are missing or not tied to the transcript.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
