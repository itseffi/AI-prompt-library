---
title: Stakeholder decision-making using TOC thinking process
category: Stakeholder Management
tags:
  - decision-making
  - stakeholders
  - theory-of-constraints
  - problem-solving
  - stakeholder-management
---
INPUTS
<provided_inputs>
- {{PROBLEM_STATEMENT}}
- {{STAKEHOLDER_INFO}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Stakeholder decision-making using TOC thinking process.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{PROBLEM_STATEMENT}}` and `{{STAKEHOLDER_INFO}}` to support stakeholder decision-making using TOC thinking processes.
- Identify and clearly state the core problem.
- Apply Evaporating Cloud:
- Define conflict.
- Identify requirements.
- Uncover assumptions.
- Challenge assumptions.
- Generate potential solutions.
- Apply Effect-Cause-Effect:
- Identify undesirable effects.
- Trace effects to causes.
- Identify root causes.
- Produce actionable recommendations and explicitly connect them to stakeholder concerns/interests.

FORMAT
Return exactly this structure:

<analysis>
1. Problem Identification:
   [Clearly state the core problem]

2. Evaporating Cloud Analysis:
   a. Conflict: [Describe the main conflict]
   b. Requirements: [List the key requirements]
   c. Assumptions: [Identify important assumptions]
   d. Challenged Assumptions: [Explain how assumptions were challenged]
   e. Potential Solutions: [List generated solutions]

3. Effect-Cause-Effect Analysis:
   a. Undesirable Effects: [List the main undesirable effects]
   b. Causes: [Explain the causes linked to each effect]
   c. Root Causes: [Identify the fundamental root causes]

4. Recommendations:
   [Provide specific, actionable recommendations based on your analysis]

5. Stakeholder Considerations:
   [Explain how your recommendations address stakeholder concerns and interests]
</analysis>

FAILURE
- Any required section in `<analysis>` is missing or materially incomplete.
- Evaporating Cloud or Effect-Cause-Effect steps are missing or not logically connected.
- Recommendations are generic, non-actionable, or not tied to stakeholder considerations.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
