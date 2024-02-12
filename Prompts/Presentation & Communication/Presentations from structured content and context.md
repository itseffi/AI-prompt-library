---
title: Presentations from structured content and context
category: Presentation & Communication
tags:
  - presentations
  - storytelling
  - product-management
  - communication
---
INPUTS
<provided_inputs>
- {{PRESENTATION_CONTENT}}
- {{ADDITIONAL_CONTEXT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Presentations from structured content and context.
Success metric:
- Produces a coherent slide narrative from provided content/context with clear logical flow.
- Uses a "What, So What, Now What?" structure (or explains gaps when unavailable).
- Delivers slide-ready outputs with concrete titles, layouts, and supporting points.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRESENTATION_CONTENT}}` and `{{ADDITIONAL_CONTEXT}}`; if information is missing, state assumptions explicitly.
- Build a clear narrative flow using "What, So What, Now What?" as the default organizing model.
- If one or more structure parts are missing in the source input, explicitly identify the gap and propose how to fill it.
- Each slide must include:
  - a descriptive, point-making title,
  - layout guidance,
  - main point with supporting points.
- Add visual/chart suggestions only when supported by provided information; do not invent data.
- Keep flow logical, audience-friendly, and suitable for direct deck production.

FORMAT
Return exactly this structure:

<presentation_plan>
<introduction>
[Purpose of the presentation and intended audience/context framing]
</introduction>

<structure_map>
- What: [How the deck defines the topic/current state]
- So What: [Why it matters; implications]
- Now What: [Recommended actions/next steps]
</structure_map>

<slides>
Slide 1: [Title]
Layout: [Layout description]
Content:
- [Main point]
  - [Supporting point 1]
  - [Supporting point 2]
Visual notes: [Chart/visual suggestion only if supported by provided inputs]

Slide 2: [Title]
Layout: [Layout description]
Content:
- [Main point]
  - [Supporting point 1]
  - [Supporting point 2]
Visual notes: [Chart/visual suggestion only if supported by provided inputs]

[Continue for all slides in logical order]
</slides>

<gaps_and_recommendations>
[Missing "What/So What/Now What" elements and specific suggestions to complete them]
</gaps_and_recommendations>

<conclusion>
[Key takeaways and clear next step/call to action]
</conclusion>
</presentation_plan>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Slides are not organized into a coherent "What, So What, Now What?" flow.
- Slide titles do not convey main points.
- Visual/chart notes include unsupported or invented data.
- Missing-structure gaps are present in input but not acknowledged with recommendations.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
