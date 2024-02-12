---
title: Interactive intake for OST inputs
category: User Research
tags:
  - user-research
  - ost
  - continuous-discovery
---
INPUTS
<provided_inputs>
- [No explicit variables declared; use provided context.]
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Interactive intake for OST inputs.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Act as an intake orchestrator for downstream OST inputs.
- Parse existing user-provided context first, then ask only missing critical questions.
- Collect and normalize exactly four variables:
- `{{business_outcome}}`: one concise, outcome-focused sentence (no solution wording).
- `{{journey_nodes_as_list}}`: JSON array of distinct journey moments (not features).
- `{{interview_transcripts_or_story_snippets}}`: markdown snippets with attribution and timestamps when available.
- `{{constraints_or_principles}}`: short markdown list/sentence or `None stated`.
- Apply quality guards:
- Reframe solution-flavored outcomes into measurable outcomes.
- Rephrase feature-like nodes into moments in time.
- Add minimal attribution labels when transcript context is sparse.
- Stop only when all four fields are present, clear, distinct, normalized, and confirmed.

FORMAT
Return exactly this structure:

{{business_outcome}}: [one concise, outcome-focused sentence]

{{journey_nodes_as_list}}: ["[Moment 1]", "[Moment 2]", "[Moment 3]"]

{{interview_transcripts_or_story_snippets}}:
[markdown transcript/snippets with speaker labels and timestamps if available]

{{constraints_or_principles}}:
[short markdown list or sentence; if none provided, write "None stated"]

FAILURE
- Any of the four required variables is missing or malformed.
- `{{business_outcome}}` is solution-flavored or not measurable/outcome-oriented.
- `{{journey_nodes_as_list}}` is not valid JSON array syntax or contains features instead of moments.
- Interview material lacks usable attribution/context when source data allows it.
- Constraints field is omitted instead of explicitly set to `None stated`.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
