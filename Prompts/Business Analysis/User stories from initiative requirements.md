---
title: User stories from initiative requirements
category: Business Analysis
tags:
  - pm
  - user-stories
  - requirements
  - business-analysis
---
INPUTS
<provided_inputs>
- {{USER_STORY_TEMPLATE}}
- {{INITIATIVE_CONTEXT}}
- {{FUNCTIONALITY_DESCRIPTION}}
</provided_inputs>

GOAL
Break initiative functionality into clear, implementable user stories using `USER_STORY_TEMPLATE`, `INITIATIVE_CONTEXT`, and `FUNCTIONALITY_DESCRIPTION`.
Success metric:
- Produces separate stories for distinct functionality/interaction units.
- Each story is self-contained, value-driven, and has testable acceptance criteria.
- Story wording follows the provided template structure.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required workflow:
  1. Read template, context, and functionality description.
  2. Decompose functionality into distinct user-value units.
  3. Draft one story per unit.
  4. Add clear, testable acceptance criteria per story.
- Follow `USER_STORY_TEMPLATE` exactly for each story.
- Keep stories implementation-ready, user-value focused, and non-duplicative.
- Ensure each story is atomic (single primary intent/outcome).
- Include a brief summary of decomposition logic and key considerations.

FORMAT
Return exactly this structure:

Here are the user stories for the described initiative:
1. <user_story>[User story 1 using the provided template, including clear acceptance criteria]</user_story>
2. <user_story>[User story 2]</user_story>
[Continue numbering for all required stories]
<summary>[Brief summary of decomposition approach and key considerations]</summary>

FAILURE
- Missing required line header, missing numbered `<user_story>` list, or missing `<summary>`.
- Stories do not follow the provided template structure.
- Stories are vague, not testable, or not grounded in provided context/functionality.
- Stories are duplicative or combine multiple primary intents into one.
- Assumptions are used but not explicitly stated.
