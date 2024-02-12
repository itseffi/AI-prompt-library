---
title: User stories with Gherkin acceptance criteria from requirements
category: Business Analysis
tags:
  - pm
  - user-stories
  - gherkin
  - requirements
  - business-analysis
---
INPUTS
<provided_inputs>
- [No explicit variables declared; use provided context.]
</provided_inputs>

GOAL
Generate INVEST-compliant, atomic user stories with Gherkin acceptance criteria from provided requirements context.
Success metric:
- Produces one or more atomic user stories aligned to persona goals and constraints.
- Each story includes deterministic happy-path and edge/negative Gherkin scenarios.
- Includes traceability from requirements to stories and acceptance criteria.
- Follows the required markdown output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required steps:
  1. Decompose requirements into distinct atomic outcomes.
  2. Draft one story per outcome.
  3. Add Gherkin acceptance criteria with one `When` and one `Then` in happy path.
  4. Add at least one edge/negative scenario per story.
  5. Complete notes and traceability mapping.
- Stories must be INVEST-compliant and persona-aligned.
- If a story would require multiple primary outcomes, split it or mark `SPLIT SUGGESTED`.
- Keep language testable and implementation-neutral (unless a technical constraint is explicitly required).
- Use `[TBD]` for critical missing info and surface it under Open Questions.

FORMAT
Return exactly this structure:

```md
Backlog Context
[Backlog Header Template fields filled]

User Story [ID-###]:
[Use Case + Gherkin happy-path scenario + Gherkin edge/negative scenario]
Notes
[Non-Functional, Instrumentation, Dependencies, Out of Scope, Open Questions]

[Repeat story blocks for each atomic outcome]

Traceability Table
[Requirement ID | Requirement Summary | Story ID(s) | AC Coverage Notes]

Validation Checklist
[All required checklist items]
```

FAILURE
- Required markdown structure is missing or malformed.
- Stories are non-atomic, non-INVEST, or not mapped to clear outcomes.
- Happy-path scenario contains more than one `When` or more than one `Then` without `SPLIT SUGGESTED`.
- Edge/negative scenario is missing for any story.
- Traceability table or validation checklist is missing.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
