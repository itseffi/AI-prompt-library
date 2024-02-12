---
title: Easy signal identification from product assumption
category: User Research
tags:
  - user-research
  - assumptions
  - validation
---
INPUTS
<provided_inputs>
- {{ASSUMPTION}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Easy signal identification from product assumption.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Design an early, efficient validation signal for `{{ASSUMPTION}}` (`We believe that ...`).
- Output must be plain text only: no XML/HTML tags, no code fences.
- Use optional context if provided (segment, function, stage, constraints, assets/access, time/budget); if missing, infer minimally and note in summary.
- Internally classify assumption lens (Desirability / Feasibility / Viability / Usability) and choose methods accordingly.
- Apply suitability rules:
- Enterprise/B2B with procurement/security: favor interviews, LOIs, security dry-runs, demos, ROI/TCO checks, RFP/API alignment; avoid fake-door/consumer funnel tactics.
- SMB SaaS: favor discovery calls, lightweight trial/offer tests, POC requests, list tests, analytics.
- Consumer: favor ad intent, waitlist conversion, community/panel, preorders, competitor-behavior proxies.
- Regulated contexts: favor standards mapping, SME/regulatory preflight, de-identified/synthetic data; avoid sensitive-data collection without approvals.
- Feasibility assumptions: favor spikes, benchmarks, vendor/data audits over user-facing tests where unnecessary.
- Quality bar for selected signal:
- Early (idea/prototype viable), cheap, attributable, decisive (quantified threshold), context-suitable, and ethical/compliant.
- Provide exactly three sections in this order: `SCRATCHPAD`, `EFFICIENT SIGNAL`, `SUMMARY`.

FORMAT
Return exactly this structure:

SCRATCHPAD
- [Signal name] — [positive evidence] — [quick capture method] — [context suitability]
- [At least 5 total lines]

EFFICIENT SIGNAL
Signal description: [clear signal]
Method: [minimal-step approach]
Suitability: [why this fits context]
Earliest stage: [Idea | Prototype | Alpha | Beta]
Participants/sample: [who/how many]
Timebox & cost: [duration and estimate]
Success threshold: [quantified pass/fail criterion]
Data captured: [metrics/notes/artifacts]
Risks/ethics: [risks and mitigations]
Next evidence rung: [single next step if positive]

SUMMARY
[3-5 sentences restating the assumption, diagnostic lens, rationale for chosen signal, and key excluded options]

FAILURE
- Output is not plain text or includes XML/HTML/code fences.
- Missing required sections or wrong section order (`SCRATCHPAD`, `EFFICIENT SIGNAL`, `SUMMARY`).
- `SCRATCHPAD` has fewer than 5 distinct signals.
- `EFFICIENT SIGNAL` misses any required line or lacks quantified success threshold.
- Selected method violates suitability/ethics constraints for the given context.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
