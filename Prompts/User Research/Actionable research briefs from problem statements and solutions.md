---
title: Actionable research briefs from problem statements and solutions
category: User Research
tags:
  - user-research
  - research-brief
  - ux
---
INPUTS
<provided_inputs>
- {{PROBLEM_STATEMENT}}
- {{PROPOSED_SOLUTION}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Actionable research briefs from problem statements and solutions.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{PROBLEM_STATEMENT}}` and `{{PROPOSED_SOLUTION}}` to produce an actionable UX research brief.
- Include and connect the following components:
- Background context.
- Scope and key risks to investigate.
- Rough research timeline.
- Research type.
- Research methods (qualitative and/or quantitative as appropriate).
- Concrete deliverables.
- Expected outcomes, learnings, and measurement plan.
- Keep recommendations specific, feasible, and aligned to decision-making needs.
- Provide rationale for chosen research type/methods/timing.

FORMAT
Return exactly this structure:

<research_brief>
## Introduction
[Brief summary of problem and proposed solution]

## Background Context
[Context and core issues]

## Scope and Risks
[What the research will cover and key risks/challenges to validate]

## Rough Timelines
[Phased timeline with approximate duration]

## Type of Research
[Evaluative, generative, exploratory, validation, etc., with rationale]

## Research Methods
[Methods, participants, and why they fit]

## Research Deliverables
[Specific outputs from the research]

## Expected Outcomes, Learnings, and Measurements
[What decisions this research should inform and how success will be measured]
</research_brief>

FAILURE
- `<research_brief>` schema is missing, malformed, or materially incomplete.
- Required brief components are missing or weakly specified.
- Methods are not aligned to the problem/solution or lack clear rationale.
- Deliverables/outcomes are generic and not decision-oriented.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
