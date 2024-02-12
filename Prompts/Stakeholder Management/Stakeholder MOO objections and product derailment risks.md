---
title: Stakeholder MOO objections and product derailment risks
category: Stakeholder Management
tags:
  - stakeholder-management
  - risk-management
  - product-strategy
  - communication
---
INPUTS
<provided_inputs>
- [No explicit variables declared; use provided context.]
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Stakeholder MOO objections and product derailment risks.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Apply MOO (Most Obvious Objection) analysis to stakeholder risk/derailment scenarios.
- First collect only essential context; ask concise follow-ups with a maximum of 5 questions total if needed.
- If sufficient context exists, produce:
- `BLUF` with top 3 stakeholder-voice MOOs, why obvious, confidence, and QBQ.
- Stakeholder objection mapping with objection type, MOO rank, QBQ, loss/gain framing, frequency x magnitude, evidence requested, counter-moves, and decision thresholds.
- Red-team drill questions, proof and pre-wire plan, executive one-slide summary, risk register, and vibe-check behaviors.
- Use plain, scannable language; label assumptions/uncertainties; prioritize obvious objections first; include numbers where possible.
- Ensure edge-case objections are covered (data quality, privacy, model eval/bias when relevant, scale/support load, contracts/channel conflict/cannibalization, change management, measurement validity).
- If context is insufficient, output only:
- A 5-question minimal follow-up.
- A clearly labeled provisional top-3 MOO guess.

FORMAT
Return exactly this structure:

If context is insufficient:
Minimal Follow-up (5 questions)
1. [question]
2. [question]
3. [question]
4. [question]
5. [question]
Provisional Top-3 MOO Guess (clearly labeled)
- [MOO 1]
- [MOO 2]
- [MOO 3]

If context is sufficient:
A) BLUF - Top 3 MOOs
- [stakeholder-voice objection + why obvious + confidence + QBQ]

B) Stakeholder Objection Map
| Stakeholder Group | Objection | Type | MOO Rank (1-5) | QBQ | Loss vs Gain | Freq x Magnitude | Evidence Asked | Counter-moves | Decision Threshold |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [row] | [row] | [row] | [row] | [row] | [row] | [row] | [row] | [row] | [row] |

C) Red-Team Drill
- [5-10 sharp questions]

D) Proof & Pre-Wire Plan
Fast proof stack:
- [test]
Artifacts:
- [artifact]
Pre-wire scripts:
- Email/Slack template (<=120 words): [text]
- 60-sec live opener: [text]
- If-they-say-X, you-say-Y snippets (top 3): [text]

E) Executive Slide (1 slide)
Title: [text]
- Why now: [text]
- Top MOO + QBQ: [text]
- Evidence to date: [text]
- Next proof step + decision gate: [text]
- Ask (people/time/budget) + trade-offs: [text]

F) Risk Register
| Risk | Trigger | Early Warning Signal | Owner | Mitigation | Kill-switch |
| --- | --- | --- | --- | --- | --- |
| [row] | [row] | [row] | [row] | [row] | [row] |

G) Vibe Check
Behaviors to avoid:
- [item]
Grounded behaviors to show:
- [item]

FAILURE
- Does not follow the conditional output path (insufficient-context vs sufficient-context).
- Missing required MOO sections (`A` through `G`) when context is sufficient.
- Objection map lacks required fields (type, rank, QBQ, evidence, threshold, counter-moves).
- Red-team, proof/pre-wire, risk register, or vibe-check sections are missing or superficial.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
