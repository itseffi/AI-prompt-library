---
title: "Stakeholder Risk Review for a Feature or PRD"
category: "Stakeholder Management"
tags:
  - stakeholder-management
  - risk-management
  - product-management
  - communication
  - internal-politics
---
INPUTS
<provided_inputs>
- [No explicit variables declared; use provided context.]
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Stakeholder Risk Review for a Feature or PRD".
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Review a feature/PRD for stakeholder and political risk before broad circulation.
- Build a Power-Interest snapshot (with named stakeholders) and include informal influencers.
- Identify stakeholders likely to feel threatened/excluded/overruled and articulate concrete objections.
- Provide mitigation guidance in two tracks:
- Document improvements (evidence, ownership, metrics, clarifications).
- 1:1 stakeholder messaging (focus, proof points, artifacts).
- Recommend exactly 3 pre-work actions before broad sharing.
- Provide framing variations for execs vs ICs and a minimal comms sequence.
- List top decision/optics risks with mitigations (pilot scope, phased rollout, sunset criteria, contingencies).
- Provide a practical readiness checklist (data, owners, dependencies, support, legal/privacy where relevant).

FORMAT
Return exactly this structure:

Power-Interest Snapshot
| Quadrant | Stakeholders |
| --- | --- |
| High Power / High Interest | [names] |
| High Power / Low Interest | [names] |
| Low Power / High Interest | [names] |
| Low Power / Low Interest | [names] |
Informal influencers: [names and why]

Stakeholder Concerns
| Stakeholder | Concern | Evidence Needed | Suggested Response |
| --- | --- | --- | --- |
| [row] | [row] | [row] | [row] |

Doc Changes
- [specific PRD/doc edit]

1:1 Messages
- [Stakeholder]: [message focus, proof points, artifacts]

Pre-Work: Top 3 Actions
1. [action]
2. [action]
3. [action]

Framing & Comms Sequence
Exec framing: [benefits, risks, ask]
IC framing: [benefits, risks, ask]
Comms sequence:
1. [step]
2. [step]
3. [step]

Risks & Mitigations
| Risk | Why it matters | Mitigation | Owner |
| --- | --- | --- | --- |
| [row] | [row] | [row] | [row] |

Readiness Checklist
- [ ] Data readiness confirmed
- [ ] Owners assigned
- [ ] Dependencies mapped
- [ ] Support plan defined
- [ ] Legal/privacy review completed (if applicable)
- [ ] [additional item]

Assumptions
- [assumption or "None"]

FAILURE
- Any required section is missing or materially incomplete.
- Fewer or more than 3 items in `Pre-Work: Top 3 Actions`.
- Stakeholder concerns are generic or lack evidence/response mapping.
- Power-Interest snapshot omits names or ignores informal influencers.
- Risks/mitigations are not actionable or lack ownership.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
