---
title: Presentation narratives from conversation transcripts
category: Presentation & Communication
tags:
  - presentations
  - storytelling
  - executive-communication
  - product-management
  - research-synthesis
---
INPUTS
<provided_inputs>
- {{CONVERSATION_TRANSCRIPTS}}
- {{PRESENTATION_TOPIC}}
- {{TARGET_AUDIENCE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Presentation narratives from conversation transcripts.
Success metric:
- Produces a coherent 3-arc presentation narrative grounded in transcript evidence.
- Tailors narrative language and emphasis to the stated target audience.
- Concludes with a clear buy-in request in Arc 3.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{CONVERSATION_TRANSCRIPTS}}`, `{{PRESENTATION_TOPIC}}`, and `{{TARGET_AUDIENCE}}`; if key context is missing, state assumptions explicitly.
- Build exactly three arcs:
  - Arc 1: Introduction and Problem Statement
  - Arc 2: Proposed Solution or Approach
  - Arc 3: Benefits and Implementation
- Ground each arc in transcript themes, points, examples, or data.
- Maintain logical transitions across arcs and audience-appropriate tone/detail.
- Include `[VISUAL]` placeholders where charts, diagrams, or evidence visuals improve clarity.
- Arc 3 must include a specific buy-in request (what approval/action is needed).
- Keep narrative scope roughly suitable for a 10-15 slide deck.

FORMAT
Return exactly this structure:

<presentation_narrative>
<arc1>
[Write the narrative for Arc 1: Introduction and Problem Statement]
</arc1>

<arc2>
[Write the narrative for Arc 2: Proposed Solution or Approach]
</arc2>

<arc3>
[Write the narrative for Arc 3: Benefits and Implementation, including the buy-in request]
</arc3>
</presentation_narrative>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Arc narratives are not grounded in provided transcripts/topic.
- No `[VISUAL]` placeholders are included.
- Arc 3 does not contain a concrete buy-in request.
- Narrative is not audience-tailored or lacks coherent transitions.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
