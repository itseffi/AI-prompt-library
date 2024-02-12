---
title: Event tracking schemas from UI and metrics requirements
category: Business Analysis
tags:
  - pm
  - business-analysis
  - analytics
  - event-tracking
  - metrics
---
INPUTS
<provided_inputs>
- {{UI_DESCRIPTION}}
- {{METRICS_AND_BEHAVIORS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Event tracking schemas from UI and metrics requirements.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Follow these task requirements:
<task_requirements>
- Identify key interactive UI elements and user actions implied by `UI_DESCRIPTION`.
- Map each proposed event to one or more items in `METRICS_AND_BEHAVIORS`.
- For each event, include only high-value properties needed for analysis and decision-making.
- Avoid duplicate or redundant events that measure the same action at the same granularity.
- Use descriptive, implementation-ready event names and property descriptions.
</task_requirements>

FORMAT
Return exactly this structure:

<event_tracking_proposal>
<event>
<name>[Event Name]</name>
<trigger>[When the event should be triggered]</trigger>
<schema>
- property1: [description]
- property2: [description]
- ...
</schema>
<justification>[Brief explanation of why this event and its properties are important for the given metrics/behaviors]</justification>
</event>
[Repeat for each proposed event]
</event_tracking_proposal>

FAILURE
- Output misses required sections, steps, or reasoning required by `<task_requirements>`.
- Required format/schema is missing, malformed, or incomplete.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
