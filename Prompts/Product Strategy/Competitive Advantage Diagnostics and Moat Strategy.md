---
title: Competitive Advantage Diagnostics and Moat Strategy
category: Product Strategy
tags:
  - strategy
  - competitive-advantage
  - moats
  - 7-powers
---
INPUTS
<provided_inputs>
- {{BUSINESS_NAME}}
- {{ONE_LINER}}
- {{STAGE}}
- {{BUSINESS_MODEL}}
- {{UNIT_ECONOMICS}}
- {{SCALE}}
- {{PRODUCT_USAGE}}
- {{DATA_IP_RESOURCES}}
- {{GTM}}
- {{COMPETITION}}
- {{CONSTRAINTS}}
- {{TIME_HORIZON}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Competitive Advantage Diagnostics and Moat Strategy.
Success metric:
- Diagnoses which of the 7 Powers are present, emerging, or absent with evidence-linked benefits and barriers.
- Provides acquisition playbooks for missing powers with concrete steps and KPIs.
- Produces a prioritized 30/60/90 plan and red-team risks with validation tests.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs; if key inputs are missing, state assumptions explicitly (do not ask questions in the output).
- For every claimed advantage, pair benefit + barrier; no barrier means no Power.
- Diagnose each of the 7 Powers as Present/Emerging/Absent with evidence and confidence.
- Provide acquisition playbooks for each Absent/Emerging power with concrete actions and KPIs.
- Include 30/60/90 actions and a red-team section with falsification tests.
- Keep claims specific, measurable, and grounded in inputs.

FORMAT
Return exactly this structure:

### A) Summary Table

| Power | Status (Present/Emerging/Absent) | Benefit | Barrier | Evidence & Metrics | Confidence | Trend (↑/→/↓) | Stage Fit |
| ----- | -------------------------------- | ------- | ------- | ------------------ | ---------: | :-----------: | --------- |

### B) Verdict (<=120 words)

[Plain-English call on sustainability of advantage.]

### C) Acquisition Playbooks (for each Absent/Emerging power)

**[Power Name]**
- Prerequisites: [List]
- Plays (3-5): [Concrete steps]
- 12-24 mo roadmap: [Milestones]
- KPIs & leading indicators: [Metrics + targets]
- Risks & countermeasures: [Bullets]
- Stop/kill criteria: [Bullets]

### D) 30/60/90

- 30 days: [Top 3 actions with owner, resources, success metric]
- 60 days: [Top 3 actions with owner, resources, success metric]
- 90 days: [Top 3 actions with owner, resources, success metric]

### E) Red Team

1. [Why this could be wrong] - [How to test]
2. [Why this could be wrong] - [How to test]
3. [Why this could be wrong] - [How to test]

FAILURE
- Any required section/table from `FORMAT` is missing, malformed, or incomplete.
- Any power marked Present/Emerging lacks a clear benefit+barrier pairing.
- Acquisition playbooks are missing for any Absent/Emerging power.
- 30/60/90 actions lack owners, resources, or success metrics.
- Red-team section lacks falsification tests.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
