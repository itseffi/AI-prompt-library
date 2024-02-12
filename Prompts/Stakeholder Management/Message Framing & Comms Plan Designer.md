---
title: Message Framing & Comms Plan Designer
category: Stakeholder Management
tags:
  - communication
  - executive-communication
  - messaging
  - stakeholder-management
---
INPUTS
<provided_inputs>
- [No explicit variables declared; use provided context.]
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Message Framing & Comms Plan Designer.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Use provided facts, audience, goal, and writing sample to design a message framing and communication plan.
- Provide 2-3 viable framing options, each with a one-line rationale tied to credibility, logic, and audience emotion.
- Produce two concise drafts in the user's natural tone:
- `ICs` draft with context, changes, actions, and timeline (`<=180` words).
- `Execs` draft with BLUF, risks/asks, and decision needed (`<=120` words).
- Include a strong subject/headline and two Slack snippets (announcement + reminder).
- Provide a mini comms plan with channel sequence, owner, timing, emphasis, and CTA.
- Include a `What to Omit` noise-reduction list and exactly 3 success signals.

FORMAT
Return exactly this structure:

Frames & Rationale
- [Frame 1]: [one-line rationale]
- [Frame 2]: [one-line rationale]
- [Frame 3 if used]: [one-line rationale]

Draft for ICs
Subject/Headline: [text]
[ICs draft <=180 words]
Slack snippet (announcement): [text]
Slack snippet (reminder): [text]

Draft for Execs
Subject/Headline: [text]
[Execs draft <=120 words]
Slack snippet (announcement): [text]
Slack snippet (reminder): [text]

Mini Comms Plan
| Step | Channel | Owner | Timing | Emphasis | CTA |
| --- | --- | --- | --- | --- | --- |
| [row] | [row] | [row] | [row] | [row] | [row] |

What to Omit
- [item]

Success Signals
1. [signal]
2. [signal]
3. [signal]

FAILURE
- Any required section is missing or materially incomplete.
- ICs draft exceeds 180 words or Execs draft exceeds 120 words.
- Missing subject/headline or missing either Slack snippet type (announcement/reminder).
- Comms plan table is missing required columns or sequence logic.
- Success Signals are not exactly three measurable indicators.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
