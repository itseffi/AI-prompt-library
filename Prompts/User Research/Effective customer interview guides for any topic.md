---
title: Effective customer interview guides for any topic
category: User Research
tags:
  - user-research
  - interviews
  - discussion-guide
---
INPUTS
<provided_inputs>
- {{TOPIC}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Effective customer interview guides for any topic.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Create a comprehensive customer interview discussion guide for `{{TOPIC}}` to support feature-development insights.
- Internally analyze topic components, interview priorities, and interview flow before writing the final guide.
- Build sections in this order:
- Introduction and warm-up.
- Current situation and workflow.
- Challenges and pain points.
- Desired outcomes and goals.
- Exploration of potential solutions.
- Wrap-up and next steps.
- Use best practices from Mom Test and Continuous Discovery Habits:
- Open-ended, non-leading, behavior-based questions.
- Focus on past experiences over hypotheticals.
- Prioritize highest-value questions first in each section.
- Use friendly professional tone, numbered questions, and optional interviewer prompts in `[brackets]`.
- Output only the final `<discussion_guide>`; do not include analysis/thinking notes.

FORMAT
Return exactly this structure:

<discussion_guide>
[Brief introduction for the interviewer, explaining the purpose of the interview and key points to remember]

1. Introduction and Warm-up
   1.1. [Question]
   1.2. [Question]
   [Additional questions as needed]

2. Current Situation and Workflow
   2.1. [Question]
   2.2. [Question]
   [Additional questions as needed]

3. Challenges and Pain Points
   3.1. [Question]
   3.2. [Question]
   [Additional questions as needed]

4. Desired Outcomes and Goals
   4.1. [Question]
   4.2. [Question]
   [Additional questions as needed]

5. Exploration of Potential Solutions
   5.1. [Question]
   5.2. [Question]
   [Additional questions as needed]

6. Wrap-up and Next Steps
   6.1. [Question]
   6.2. [Question]
   [Additional questions as needed]
</discussion_guide>

FAILURE
- `<discussion_guide>` schema is missing, malformed, or materially incomplete.
- Required sections are missing or question numbering/order is inconsistent.
- Questions are leading, hypothetical-first, or not behavior-based.
- Questions are not prioritized by importance within each section.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
