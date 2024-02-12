---
title: "Map power dynamics before meetings"
category: "Stakeholder Management"
tags:
  - stakeholders
  - power-dynamics
  - meetings
  - communication
---
INPUTS
<provided_inputs>
- {{MEETING_DETAILS}}
- {{ATTENDEES_INFO}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Map power dynamics before meetings".
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{MEETING_DETAILS}}` and `{{ATTENDEES_INFO}}` to map meeting-specific power dynamics.
- Identify formal hierarchy, informal influence signals, alliances/conflicts, and each attendee's stake in outcomes.
- Rank attendees by influence in this meeting context.
- Identify decision-makers, influencers, power imbalances, and likely conflict points.
- Provide actionable strategies to navigate dynamics during the meeting.
- If information is insufficient for any claim, explicitly state the uncertainty.

FORMAT
Return exactly this structure:

<power_dynamics_analysis>
<power_map>
[List attendees in order of influence, with brief notes on their power sources]
</power_map>

<key_observations>
[Bullet points of important observations about the power dynamics]
</key_observations>

<strategic_recommendations>
[Bullet points of strategies to navigate the power dynamics effectively]
</strategic_recommendations>
</power_dynamics_analysis>

FAILURE
- Any required section in `<power_dynamics_analysis>` is missing or materially incomplete.
- Influence ranking is not meeting-contextual or lacks power-source rationale.
- Recommendations are generic or not tied to identified dynamics/conflicts.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
