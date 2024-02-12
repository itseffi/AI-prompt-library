---
title: Actionable customer interview guides from research topics
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
Produce a high-quality deliverable for: Actionable customer interview guides from research topics.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Create a comprehensive customer interview discussion guide for `{{TOPIC}}`.
- Follow Mom Test and Continuous Discovery Habits principles:
- Open-ended, behavior-based questions.
- Focus on past experiences over hypotheticals.
- No leading or biased phrasing.
- Cover current workflow, pain points, outcomes, and usage context.
- Structure the guide in sections:
- Introduction and warm-up.
- Current situation and workflow.
- Challenges and pain points.
- Desired outcomes and goals.
- Exploration of potential solutions (without pitching).
- Wrap-up and next steps.
- Within each section:
- Number all questions.
- Prioritize the most important questions first.
- Include concise interviewer prompts in `[brackets]` where useful.
- Start with a brief interviewer introduction and key reminders.

FORMAT
Return exactly this structure:

<discussion_guide>
[Brief interviewer introduction: interview purpose and key reminders]

## Introduction and Warm-Up
1. [Question]
[Interviewer prompt in brackets if needed]

## Current Situation and Workflow
1. [Question]
[Interviewer prompt in brackets if needed]

## Challenges and Pain Points
1. [Question]
[Interviewer prompt in brackets if needed]

## Desired Outcomes and Goals
1. [Question]
[Interviewer prompt in brackets if needed]

## Exploration of Potential Solutions
1. [Question]
[Interviewer prompt in brackets if needed]

## Wrap-Up and Next Steps
1. [Question]
[Interviewer prompt in brackets if needed]
</discussion_guide>

FAILURE
- `<discussion_guide>` schema is missing, malformed, or materially incomplete.
- Required sections are missing or questions are not numbered/prioritized.
- Questions are leading, hypothetical-first, or not behavior-based.
- Guide does not cover workflow, pain points, outcomes, and context.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
