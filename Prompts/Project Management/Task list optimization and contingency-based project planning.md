---
title: Task list optimization and contingency-based project planning
category: Project Management
tags:
  - project-management
  - planning
  - scheduling
  - risk-management
---
INPUTS
<provided_inputs>
- {{TASK_LIST}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Task list optimization and contingency-based project planning.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze and optimize `{{TASK_LIST}}` by identifying dependencies, gaps, and ambiguities.
- Add missing tasks needed for completion and clarify ambiguous items.
- Sequence tasks for efficiency, highlight critical path, and assign rough durations.
- Identify resource constraints and opportunities for parallel execution.
- Build contingency plans with blockers, workarounds, and buffers.
- Define decision milestones with go/no-go criteria and metrics.
- Include a brief explanation of sequencing and key decisions.

FORMAT
Return exactly this structure:

<optimized_plan>
  <task_sequence>
  [Sequenced tasks including dependencies, rough durations, critical path markers, and any added tasks]
  </task_sequence>
  <clarifications>
  [Clarifications for ambiguous tasks and questions if needed]
  </clarifications>
  <contingency_plans>
  [Potential blockers with contingency actions and buffers]
  </contingency_plans>
  <decision_framework>
  [Milestones with go/no-go criteria and metrics]
  </decision_framework>
</optimized_plan>

<explanation>
[Brief reasoning for sequence, added tasks, and key decisions]
</explanation>

FAILURE
- Any required section (`<optimized_plan>` with its child tags, and `<explanation>`) is missing or materially incomplete.
- Task sequence lacks dependencies, sequencing logic, or critical path indicators.
- Contingencies or decision criteria are missing or not actionable.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
