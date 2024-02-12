---
title: "Structured product hypotheses from product problems"
category: "Decision Making"
tags:
  - pm
  - decision-making
  - experimentation
  - hypotheses
  - product
---
INPUTS
<provided_inputs>
- {{PRODUCT_PROBLEM}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Structured product hypotheses from product problems".
Success metric:
- Produces a clear, testable product hypothesis directly tied to the provided problem.
- Includes a measurable plan to evaluate success with explicit metrics and thresholds.
- Covers all required hypothesis-formation steps before finalizing the hypothesis.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT_PROBLEM}}`; if details are missing, state assumptions explicitly.
- Execute all six steps: experiment goal, draft hypothesis, specificity check, measurement plan, validate/refine, narrative framing.
- Draft hypothesis must include all five components: Action, Outcome, Direction, Users, Conditions.
- Keep outcomes measurable; avoid vague terms (for example: "better", "improve") without quantification.
- Ensure the final hypothesis and metrics are realistic and testable in product-experiment contexts.

FORMAT
Return exactly this structure:

<experiment_goal>
[User problem and proposed change]
</experiment_goal>

<hypothesis_draft>
[Action] will cause [Outcome] to [Direction] for [Users] under [Conditions].
</hypothesis_draft>

<specificity_check>
- Action clarity: [Pass/Fail + note]
- Outcome clarity: [Pass/Fail + note]
- Direction clarity: [Pass/Fail + note]
- Users clarity: [Pass/Fail + note]
- Conditions clarity: [Pass/Fail + note]
</specificity_check>

<measurement_plan>
- Primary metric: [Metric + baseline + target change + timeframe]
- Secondary metrics: [Metric list]
- Data collection: [How/where measured]
- Guardrails: [Risk metrics to monitor]
</measurement_plan>

<validation_and_refinement>
- Clarity gaps found: [List]
- Refinements made: [List]
</validation_and_refinement>

<narrative_framing>
[Short story-style framing linking problem -> change -> expected outcome -> evidence of success]
</narrative_framing>

<hypothesis>
Currently, [user] is experiencing [problem].
We believe that by [change], we'll see [outcome].
We'll know we're right when [metric] changes by [amount].
</hypothesis>

<explanation>
[Brief explanation of why this hypothesis fits the product problem and framework]
</explanation>

FAILURE
- Any required section in `FORMAT` is missing, malformed, or incomplete.
- Hypothesis draft omits any of the five required components.
- Measurement plan lacks metric, target change, or timeframe.
- Final `<hypothesis>` does not follow the required three-line template.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
