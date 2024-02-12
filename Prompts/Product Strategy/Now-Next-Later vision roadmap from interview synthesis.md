---
title: Now-Next-Later vision / roadmap from interview synthesis
category: Product Strategy
tags:
  - interviews
  - research-synthesis
  - product-strategy
  - roadmapping
  - vision
---
INPUTS
<provided_inputs>
- {{TRANSCRIPT}}
- Optional: {{CONTEXT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Now-Next-Later vision / roadmap from interview synthesis.
Success metric:
- Produces a Now/Next/Later roadmap grounded in transcript evidence.
- Distinguishes needs, symptoms, solutions, and underlying drivers with citations.
- Limits items to what is supported by the transcript.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{TRANSCRIPT}}` (and optional `{{CONTEXT}}`); if evidence is missing, do not infer.
- Output exactly three sections: **Now**, **Next**, **Later**.
- Each section contains 2–4 items (or fewer if evidence is insufficient).
- Each item must include: Need, Symptom, Proposed solution (if mentioned), Underlying driver, Evidence (quote/paraphrase).
- Use direct quotes <= 20 words or precise paraphrases with speaker/timestamp if available.
- If a need spans horizons, place it where it becomes critical and note cross-horizon relevance.

FORMAT
Return exactly this structure:

**Now**
1. Need: [What]
   - Symptom: [Signal]
   - Proposed solution: [How, if mentioned]
   - Underlying driver: [Why]
   - Evidence: "[Quote <=20 words]" (Speaker, timestamp) or [Paraphrase + attribution]
[2–4 items or fewer if evidence is insufficient]

**Next**
1. Need: [What]
   - Symptom: [Signal]
   - Proposed solution: [How, if mentioned]
   - Underlying driver: [Why]
   - Evidence: "[Quote <=20 words]" (Speaker, timestamp) or [Paraphrase + attribution]
[2–4 items or fewer if evidence is insufficient]

**Later**
1. Need: [What]
   - Symptom: [Signal]
   - Proposed solution: [How, if mentioned]
   - Underlying driver: [Why]
   - Evidence: "[Quote <=20 words]" (Speaker, timestamp) or [Paraphrase + attribution]
[2–4 items or fewer if evidence is insufficient]

FAILURE
- Any required section in `FORMAT` is missing or malformed.
- Items are missing required fields (Need, Symptom, Proposed solution, Underlying driver, Evidence).
- Evidence is missing or exceeds the 20-word quote limit.
- Items are inferred without transcript evidence.
