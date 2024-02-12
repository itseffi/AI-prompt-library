---
title: UX edge cases from product briefs
category: Business Analysis
tags:
  - pm
  - ux
  - design
  - edge-cases
  - business-analysis
---
INPUTS
<provided_inputs>
- {{PRODUCT_BRIEF}}
</provided_inputs>

GOAL
Identify UX edge cases from `PRODUCT_BRIEF` and define expected behavior for each scenario.
Success metric:
- Produces a comprehensive scenario set (target 15-20 unique scenarios).
- Covers diverse user types, contexts, failures, accessibility, and security/privacy considerations.
- Defines clear, testable expected behavior per scenario.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip scenario classes:
  - user-type differences,
  - context/device variations,
  - error/misuse flows,
  - system/network failures,
  - integrations/dependencies,
  - performance/load behavior,
  - security/privacy edge cases,
  - accessibility interactions.
- Keep each scenario concrete and distinct (avoid duplicates).
- Define expected behavior in product terms (clear response, recovery path, and user feedback when relevant).
- If the brief is missing specifics, state assumptions explicitly.

FORMAT
Return exactly this structure:

<analysis>
Based on the product brief, here are the potential scenarios and their expected behaviors:

| Scenario | Expected Behavior |
|----------|-------------------|
| [Scenario 1] | [Expected Behavior 1] |
| [Scenario 2] | [Expected Behavior 2] |
| ... | ... |
| [Scenario n] | [Expected Behavior n] |

</analysis>

FAILURE
- Required schema is missing or malformed.
- Fewer than 15 scenarios unless explicitly constrained by provided brief.
- Scenario coverage is narrow (missing key classes like accessibility, failures, or security/privacy).
- Expected behaviors are vague, non-testable, or not tied to scenario conditions.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
