---
title: Engineering Problem Solving and Solution Structuring
category: Technical
tags:
  - engineering
  - problem-solving
  - solution-design
  - tradeoff-analysis
  - technical
---
INPUTS
<provided_inputs>
- {{PROBLEM_TO_SOLVE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Engineering Problem Solving and Solution Structuring.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{PROBLEM_TO_SOLVE}}` and produce a structured engineering solution assessment.
- Provide:
- Problem overview.
- Key challenges.
- Three distinct solution options.
- Pros/cons analysis for each solution.
- One additional/hybrid solution.
- Final recommendation with rationale.
- Each required section must contain at least four detailed, thoughtful sentences.
- Keep recommendations technically grounded, explicit about trade-offs, and practical for implementation.

FORMAT
Return exactly this structure:

<problem_overview>[Overview of the problem]</problem_overview>
<challenges>[Key challenges in solving the problem]</challenges>
<solution1>[First potential solution]</solution1>
<solution2>[Second potential solution]</solution2>
<solution3>[Third potential solution]</solution3>
<solution1_analysis>[Analysis of pros and cons of Solution 1]</solution1_analysis>
<solution2_analysis>[Analysis of pros and cons of Solution 2]</solution2_analysis>
<solution3_analysis>[Analysis of pros and cons of Solution 3]</solution3_analysis>
<additional_solution>[Additional or hybrid solution]</additional_solution>
<recommendation>[Final recommendation on the best approach]</recommendation>

FAILURE
- Any required section is missing, malformed, or materially incomplete.
- Any required section has fewer than four sentences.
- Solutions are redundant, non-distinct, or lack trade-off analysis.
- Recommendation does not clearly justify why one approach is preferred.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
