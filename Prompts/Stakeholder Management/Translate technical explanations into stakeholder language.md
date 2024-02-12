---
title: Technical Translation and Stakeholder Communication
category: Stakeholder Management
tags:
  - stakeholder-management
  - technical-communication
  - product-management
  - decision-making
---
INPUTS
<provided_inputs>
- {{TECHNICAL_EXPLANATION}}
- {{STAKEHOLDER_TYPE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Technical Translation and Stakeholder Communication.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Translate `{{TECHNICAL_EXPLANATION}}` for `{{STAKEHOLDER_TYPE}}` into clear, decision-ready language.
- Preserve core technical meaning while reducing jargon and using relatable explanations where helpful.
- Explicitly cover:
- Overview of the technical situation.
- Business impact in stakeholder terms.
- Important considerations (risks, benefits, decisions).
- Likely stakeholder questions with direct answers.
- Recommended next steps.
- Include a brief glossary only for unavoidable technical terms.
- Final output must include only `<simplified_explanation>` and `<glossary>`.

FORMAT
Return exactly this structure:

<simplified_explanation>
1. Overview: [Brief description of the technical situation]
2. Business Impact: [Key implications for the stakeholder]
3. Important Considerations: [Risks, benefits, or decisions to understand]
4. Stakeholder Questions and Answers:
   Q1: [Likely question 1]
   A1: [Clear answer to question 1]
   Q2: [Likely question 2]
   A2: [Clear answer to question 2]
   [Add more Q&A pairs as needed]
5. Next Steps: [Recommended actions, if applicable]
</simplified_explanation>

<glossary>
- Term 1: [Brief definition]
- Term 2: [Brief definition]
[Add more terms as needed]
</glossary>

FAILURE
- `<simplified_explanation>` or `<glossary>` is missing, malformed, or materially incomplete.
- Explanation is still jargon-heavy for the specified stakeholder type.
- Q&A section is missing or does not address likely stakeholder concerns.
- Translation loses critical risks/implications from the original technical content.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
