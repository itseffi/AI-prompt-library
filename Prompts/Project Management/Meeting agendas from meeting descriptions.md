---
title: "Meeting agendas from meeting descriptions"
category: "Project Management"
tags:
  - meetings
  - facilitation
  - planning
  - productivity
---
INPUTS
<provided_inputs>
- {{MEETING_DESCRIPTION}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Meeting agendas from meeting descriptions".
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Build a meeting preparation output from `{{MEETING_DESCRIPTION}}` that includes:
- A clear purpose statement for the meeting.
- A structured agenda with allocated time per topic and key questions per topic.
- A practical process/flow for running the meeting to achieve the stated purpose.
- Internally reason from meeting goals, stakeholders, and constraints; return only the required final sections.

FORMAT
Return exactly this structure:

<purpose>
[Clear and concise purpose statement]
</purpose>

<agenda>
1. [Agenda Topic 1] - [Allocated Time]
Key Questions:
- [Question 1]
- [Question 2]
...
2. [Agenda Topic 2] - [Allocated Time]
Key Questions:
- [Question 1]
- [Question 2]
...
[Additional agenda topics]
</agenda>

<process>
[Suggested process and flow for the meeting]
</process>

FAILURE
- Any required section (`<purpose>`, `<agenda>`, `<process>`) is missing or materially incomplete.
- Agenda items do not include both time allocation and key questions.
- Meeting flow/process is generic and not tied to the stated purpose.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
