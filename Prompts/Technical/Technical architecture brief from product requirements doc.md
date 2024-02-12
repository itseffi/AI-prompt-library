---
title: Technical architecture brief from product requirements doc
category: Technical
tags:
  - software-architecture
  - startup-cto
  - systems-design
  - risk-management
  - technical
---
INPUTS
<provided_inputs>
- {{PRD}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Technical architecture brief from product requirements doc.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Create a comprehensive Technical Architecture Brief from `{{PRD}}` suitable for startup execution.
- Include and reason through all required sections:
- `System Context Diagram`
- Bounded contexts.
- Context interactions.
- Third-party integrations (APIs/SaaS/data pipelines).
- `Component Architecture`
- Monolith vs microservices trade-off.
- Recommended architecture with justification.
- Data flow, schema, and caching strategy.
- Database choice rationale (relational/NoSQL/hybrid).
- `Technology Stack Rationale`
- Frontend/backend framework recommendations with rationale.
- Infrastructure approach (cloud/on-prem/hybrid).
- Containerization and CI/CD strategy.
- `Risk Mitigation Plan`
- Failure modes and single points of failure.
- Redundancy and resilience strategies.
- High-level compute/storage cost projections aligned to growth.
- Keep recommendations tied to the PRD and explicitly state assumptions when PRD details are missing.

FORMAT
Return exactly this structure:

<Technical_Architecture_Brief>
<System_Context_Diagram>
[Content for this section]
</System_Context_Diagram>

<Component_Architecture>
[Content for this section]
</Component_Architecture>

<Technology_Stack_Rationale>
[Content for this section]
</Technology_Stack_Rationale>

<Risk_Mitigation_Plan>
[Content for this section]
</Risk_Mitigation_Plan>
</Technical_Architecture_Brief>

FAILURE
- `<Technical_Architecture_Brief>` wrapper or any required section is missing/malformed/materially incomplete.
- Recommendations are generic and not traceable to the provided PRD.
- Architecture choice lacks explicit trade-off analysis (monolith vs microservices).
- Risk plan lacks concrete failure modes, mitigation strategy, or cost-growth framing.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
