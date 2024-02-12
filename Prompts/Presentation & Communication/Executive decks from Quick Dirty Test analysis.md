---
title: Executive decks from Quick Dirty Test analysis
category: Presentation & Communication
tags:
  - executive-communication
  - decision-support
  - hypothesis-testing
  - risk-analysis
  - quick-dirty-test
---
INPUTS
<provided_inputs>
- {{SLIDE_DECK_CONTEXT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Executive decks from Quick Dirty Test analysis.
Success metric:
- Identifies critical assumptions and failure modes that executives would scrutinize.
- Provides risk-dimensioning analyses and decision-driving questions.
- Includes an executive-ready summary with practical deck-improvement recommendations.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{SLIDE_DECK_CONTEXT}}`; if information is missing, state assumptions explicitly.
- Apply Quick Dirty Test logic:
  - What must be true for the hypothesis/investment to succeed?
  - How could the investment fail or "blow up"?
- Prioritize items that materially affect executive go/no-go decisions.
- Keep outputs concise, evidence-oriented, and directly usable for deck revisions.

FORMAT
Return exactly this structure:

<qdt_analysis>
<key_assumptions>
[List the key assumptions here, one per line]
</key_assumptions>

<potential_risks>
[List the potential risks or ways the investment could fail, one per line]
</potential_risks>

<necessary_analyses>
[List the analyses needed to support or reject the investment, one per line]
</necessary_analyses>

<key_questions>
[List the key questions to dimension the risks, one per line]
</key_questions>
</qdt_analysis>

<summary>
[Brief findings summary and recommendations to strengthen the executive deck]
</summary>

FAILURE
- `<qdt_analysis>` or `<summary>` is missing, malformed, or incomplete.
- Any required subsection in `<qdt_analysis>` is missing.
- Analysis is not executive-decision oriented (missing investment belief/failure logic).
- Recommendations are generic and not actionable for deck improvement.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
