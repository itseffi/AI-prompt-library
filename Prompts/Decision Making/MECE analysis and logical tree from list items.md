---
title: "MECE analysis and logical tree from list items"
category: "Decision Making"
tags:
  - pm
  - decision-making
  - mece
  - structured-thinking
  - frameworks
---
INPUTS
<provided_inputs>
- {{LIST_OF_ITEMS}}
</provided_inputs>

GOAL
Evaluate `LIST_OF_ITEMS` for MECE quality and produce a logical tree that resolves overlaps/gaps.
Success metric:
- Clearly assesses mutual exclusivity and collective exhaustiveness.
- Identifies concrete overlaps and coverage gaps (if any).
- Produces a coherent tree structure reflecting corrected grouping logic.
- Follows the required output schema exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps:
  1. Test pairwise overlap (mutual exclusivity).
  2. Test coverage gaps (collective exhaustiveness).
  3. Propose corrected structure and hierarchy.
- Keep conclusions grounded in the provided list; avoid unrelated frameworks unless necessary.
- If ambiguity exists in item definitions, state assumptions explicitly.
- Provide concise rationale, not hidden/internal chain-of-thought.

FORMAT
Return exactly this structure:

<analysis>
<mutual_exclusivity_assessment>
[State whether items are mutually exclusive, with specific overlap examples where relevant]
</mutual_exclusivity_assessment>
<collective_exhaustiveness_assessment>
[State whether items are collectively exhaustive, with specific gap examples where relevant]
</collective_exhaustiveness_assessment>
<key_issues>
[Concise list of overlap issues and/or coverage gaps]
</key_issues>
</analysis>

<answer>
<mece_conclusion>[MECE status: Fully MECE | Not MECE | Partially MECE]</mece_conclusion>
<logical_tree>
[Hierarchical tree showing corrected structure and item placement]
</logical_tree>
</answer>

FAILURE
- Required schema sections are missing or malformed.
- Mutual exclusivity or collective exhaustiveness assessment is absent.
- Logical tree is missing, unclear, or inconsistent with analysis findings.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
