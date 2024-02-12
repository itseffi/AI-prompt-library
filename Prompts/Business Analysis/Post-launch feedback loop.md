---
title: Post-launch feedback loop
category: Business Analysis
tags:
  - pm
  - feedback-loop
  - iteration
  - post-launch
  - continuous-improvement
  - business-analysis
---
INPUTS
<provided_inputs>
- {{CURRENT_PROCESS}}
- {{PRODUCT_CONTEXT}}
- {{LAUNCH_TIMELINE}}
- {{TEAM_STRUCTURE}}
- {{AVAILABLE_DATA_SOURCES}}
</provided_inputs>

GOAL
Design a complete post-launch feedback loop system that turns product signals into prioritized iteration decisions.
Success metric:
- Defines checkpoint cadence with clear purpose and decision outputs.
- Specifies what to measure, how to synthesize signals, and how to prioritize action.
- Connects learnings to roadmap iteration and team operating rituals.
- Follows the required schema exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Keep recommendations grounded in `CURRENT_PROCESS`, `PRODUCT_CONTEXT`, `LAUNCH_TIMELINE`, `TEAM_STRUCTURE`, and `AVAILABLE_DATA_SOURCES`.
- Do not skip required analysis layers:
  - Current-state audit (gaps, latency, silos)
  - Time-based checkpoints (week 1, month 1, month 3, month 6, month 12)
  - Measurement framework (quantitative, qualitative, behavioral, technical)
  - Retrospective and learning capture process
  - Iteration planning integration and triage model
- For each checkpoint, define:
  - key questions,
  - data sources,
  - success criteria,
  - review meeting structure and outputs.
- Include both leading and lagging indicators with definitions, targets, source systems, and review cadence.
- Ensure triage rules are operational (SLA, owner, scoring logic, planning window).

FORMAT
Return exactly this structure:

<feedback_loop_framework>
<current_state_assessment>
[Existing feedback mechanisms, identified gaps, latency issues, and organizational silos/blockers]
</current_state_assessment>

<checkpoint_calendar>
<week_1_checkpoint>[Timeline, primary focus, key questions, data sources, success criteria, meeting/review details]</week_1_checkpoint>
<month_1_checkpoint>[Timeline, primary focus, key questions, data sources, success criteria, meeting/review details]</month_1_checkpoint>
<month_3_checkpoint>[Timeline, primary focus, key questions, data sources, success criteria, meeting/review details]</month_3_checkpoint>
<month_6_checkpoint>[Timeline, primary focus, key questions, data sources, success criteria, meeting/review details]</month_6_checkpoint>
<month_12_checkpoint>[Timeline, primary focus, key questions, data sources, success criteria, meeting/review details]</month_12_checkpoint>
</checkpoint_calendar>

<measurement_framework>
<quantitative_metrics>
[Leading indicators table/list + lagging indicators table/list + technical health indicators with definition, target, source, frequency]
</quantitative_metrics>
<qualitative_insights>
[User research schedule, support analysis method, sales/marketing feedback integration cadence]
</qualitative_insights>
<behavioral_monitoring>
[Unexpected pattern detection, workaround identification, feature misuse tracking]
</behavioral_monitoring>
</measurement_framework>

<retrospective_process>
<template>
[Structured template covering goals/hypotheses, validated and invalidated assumptions, surprises, key learnings, user quotes, quantitative highlights, recommendations]
</template>
<documentation_location>[Where learnings are stored and how they are indexed/retrieved]</documentation_location>
<review_meeting_structure>[Attendees, duration, pre-work, agenda, outputs]</review_meeting_structure>
</retrospective_process>

<iteration_planning_integration>
<triage_framework>
**Critical Issues (Address Immediately):**
- Definition: [What qualifies]
- Response time: [SLA]
- Decision maker: [Who can approve]

**High Priority (Next Sprint):**
- Definition: [What qualifies]
- Scoring formula: [How prioritized]
- Review cadence: [How often re-evaluated]

**Medium Priority (Next Quarter):**
- Definition: [What qualifies]
- Planning cycle: [When incorporated into roadmap]

**Low Priority (Backlog):**
- Definition: [What qualifies]
- Archive criteria: [When to deprioritize]
</triage_framework>
</iteration_planning_integration>
</feedback_loop_framework>

FAILURE
- Any required top-level section is missing or malformed.
- Checkpoint plan lacks timeline, data sources, success criteria, or decision outputs.
- Measurement framework lacks explicit metrics, definitions, or cadence.
- Triage/iteration process is vague or non-operational.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
