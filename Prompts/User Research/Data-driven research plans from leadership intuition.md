---
title: Data-driven research plans from leadership intuition
category: User Research
tags:
  - user-research
  - research-planning
  - product-strategy
---
INPUTS
<provided_inputs>
- {{COMPANY_CONTEXT}}
- {{INTUITION}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Data-driven research plans from leadership intuition.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Convert `{{INTUITION}}` into an evidence-based research plan grounded in `{{COMPANY_CONTEXT}}`.
- Include:
- Intuition summary with explicit bias/assumption check.
- Prioritized key assumptions affecting feature success.
- 3-5 measurable research objectives tied to assumptions.
- Mixed quantitative + qualitative methods with rationale per objective.
- Validation/refutation success metrics aligned to business goals.
- Risks/challenges with mitigation strategies.
- Realistic milestone-based timeline.
- Keep analysis objective and decision-oriented (validate, refute, or partially support intuition).

FORMAT
Return exactly this structure:

<research_plan>
1. Executive Summary: [brief decision-oriented summary]
2. Analysis of Intuition: [key points + potential biases/assumptions]
3. Key Assumptions: [prioritized assumptions]
4. Research Objectives: [3-5 measurable objectives]
5. Research Methods: [mixed methods + why each fits]
6. Success Metrics: [clear validation/refutation thresholds]
7. Potential Challenges and Mitigation Strategies: [risk -> mitigation]
8. Proposed Timeline: [milestones and duration]
9. Conclusion: [how findings will inform go/no-go or iteration decisions]
</research_plan>

FAILURE
- `<research_plan>` schema is missing, malformed, or materially incomplete.
- Research objectives are not measurable or not tied to key assumptions.
- Methods do not include both quantitative and qualitative approaches (unless explicitly justified by context).
- Success metrics are vague and lack decision thresholds.
- Timeline lacks milestones or is not feasible for proposed methods.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
