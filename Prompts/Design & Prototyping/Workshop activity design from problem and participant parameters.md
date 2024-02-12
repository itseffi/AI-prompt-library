---
title: "Workshop activity design from problem and participant parameters"
category: "Design & Prototyping"
tags:
  - workshops
  - facilitation
  - brainstorming
  - product
  - ux
---
INPUTS
<provided_inputs>
- {{PROBLEM}}
- {{PARTICIPANTS}}
- {{TIME_AVAILABLE}}
- {{PLATFORM}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Workshop activity design from problem and participant parameters".
Success metric:
- Produces 3-5 distinct workshop activity variants tailored to problem, participants, time, and platform.
- Each variant is facilitator-ready, includes exact timing, and is feasible within `{{TIME_AVAILABLE}}`.
- Variants include practical tradeoffs, inclusion mechanics, and clear runbooks.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs; if any input is incomplete, state explicit assumptions per variant.
- Generate 3-5 distinct variants.
- Do not use XML or JSON anywhere in the response.
- For each variant, total duration must be `<= {{TIME_AVAILABLE}}`, and timeline minute ranges must sum exactly to the stated total.
- Adapt mechanics by participant size:
  - `<=8`: whole-group flow with silent ideation first.
  - `9-20`: pods of 3-5 with rotating roles/report-outs.
  - `>20`: swarm + pods (4-6) + gallery walk + synthesis.
- Adapt logistics by platform:
  - `remote/hybrid`: breakout choreography and linked board flow.
  - `in-person`: room setup, physical materials, visible timing controls.
- Include inclusion and bias-mitigation mechanisms (silent write, timeboxing, anonymous voting, speaker rotation, accessibility notes).
- Include practical Miro runbook guidance for intermediate users; if in-person-only with no Miro, write `Not applicable`.
- Across the full set of variants, include at least:
  - one rapid ideation pattern,
  - one prioritization pattern,
  - one synthesis pattern.
- Keep language facilitator-ready and operational.

FORMAT
Return exactly this structure:

Here are multiple workshop activity variants designed to address the given problem(s):

### Variant X: *[Activity Name]*
**Assumptions**
- [Assumptions]

**Overview (2-3 sentences)**
- [Overview]

**Rationale**
- [Why it fits problem, participants, time, platform]

**Duration**
- **Total minutes:** [N]

**Timeline (minute-by-minute; sums to total)**
- 00:00-00:XX — [Step]
- 00:XX-00:YY — [Step]

**Facilitator Process**
1. [Concrete facilitator step with timing]
2. [Concrete facilitator step with timing]
- **Scaling notes:** [<=8 | 9-20 | >20 adaptations]
- **If time slips +/-10%:** [What to shorten/extend]

**Participant Process**
1. [What participants do]
2. [What participants produce/decide]

**Miro Setup & Runbook (intermediate)**
- [Board prep, frames, breakouts, timer, voting, mapping, export]
- [If not applicable: "Not applicable"]

**Inputs (bring to the workshop)**
- [Inputs]

**Outputs (created by the activity)**
- [Outputs]

**Pros**
- [Pros]

**Cons (with mitigations)**
- [Cons + mitigation]

[Repeat full variant structure for 3-5 variants]

FAILURE
- Opening line is missing or different from required text.
- Fewer than 3 or more than 5 variants are provided.
- Any variant exceeds `{{TIME_AVAILABLE}}` or timeline math does not sum to stated total.
- Output contains XML or JSON.
- Variant sections are missing required headings/items from `FORMAT`.
- Participant-size and platform adaptations are not reflected.
- Miro runbook is missing (or not marked `Not applicable` when appropriate).
- Required pattern coverage across the set (rapid ideation, prioritization, synthesis) is incomplete.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
