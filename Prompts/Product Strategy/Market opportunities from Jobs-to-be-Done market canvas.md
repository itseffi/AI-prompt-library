---
title: Market opportunities from Jobs-to-be-Done market canvas
category: Product Strategy
tags:
  - jobs-to-be-done
  - market-definition
  - customer-insight
  - product-strategy
---
INPUTS
<provided_inputs>
- {{PRODUCT_OR_SERVICE}}
- {{USER_INPUT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Market opportunities from Jobs-to-be-Done market canvas.
Success metric:
- Guides the user through all 8 JTBD canvas steps with clear prompts.
- Keeps responses tied to provided `{{USER_INPUT}}` and the product context.
- Ends with a concise summary prompt that reflects the completed canvas.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT_OR_SERVICE}}` and `{{USER_INPUT}}`; if context is missing, state assumptions explicitly.
- Ask for user input at each of the 8 JTBD canvas steps.
- Provide a brief explanation before each step’s prompt.
- Require the user to answer within the specified `<stepN>` tags.
- End by requesting a `<summary>` that synthesizes the full canvas.
- Remind the user to use `{{USER_INPUT}}` when answering.

FORMAT
Return exactly this structure:

<step1>
[Prompt + explanation for Traditional Market Definition]
</step1>

<step2>
[Prompt + explanation for Job Executor Determination]
</step2>

<step3>
[Prompt + explanation for Abstracted Job Executor]
</step3>

<step4>
[Prompt + explanation for Job Executor Documentation]
</step4>

<step5>
[Prompt + explanation for Product Function Analysis]
</step5>

<step6>
[Prompt + explanation for Complementary Product Analysis]
</step6>

<step7>
[Prompt + explanation for Job Statement Abstraction]
</step7>

<step8>
[Prompt + explanation for Final Job Documentation]
</step8>

<summary>
[Prompt asking the user to summarize the completed canvas]
</summary>

FAILURE
- Any required step tag in `FORMAT` is missing, malformed, or incomplete.
- Prompts do not request user responses within the correct `<stepN>` tags.
- User is not reminded to use `{{USER_INPUT}}` for responses.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
