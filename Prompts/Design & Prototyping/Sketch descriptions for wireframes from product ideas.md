---
title: Sketch descriptions for wireframes from product ideas
category: Design & Prototyping
tags:
  - pm
  - ux
  - flows
  - design
  - prototyping
  - wireframes
---
INPUTS
<provided_inputs>
- {{PRODUCT_IDEA}}
- {{ADDITIONAL_DETAILS}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Sketch descriptions for wireframes from product ideas.
Success metric:
- Produces 3-5 detailed sketch descriptions covering distinct product flows/aspects.
- Each sketch includes layout, interaction flow, friction reduction, and design variations.
- Output is specific enough for a visual designer to create wireframes/mockups directly.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT_IDEA}}` and `{{ADDITIONAL_DETAILS}}`; if details are missing, state assumptions explicitly.
- Generate 3-5 sketches, each focused on a distinct flow/aspect (not minor variants of the same screen).
- For each sketch include:
  - Title/identifier
  - What the sketch represents
  - Key UI elements and placement
  - User flow and interaction points
  - At least one meaningful variation/alternative
- Incorporate user-centric design, friction reduction, onboarding considerations, consistency, and scalability.
- Do not restate input prompts verbatim in the output.

FORMAT
Return exactly this structure:

<sketch_descriptions>
<sketch>
<title>[Sketch title]</title>
<description>[What this sketch represents]</description>
<key_elements_and_layout>[Key elements and placement]</key_elements_and_layout>
<user_flow_and_interactions>[Start point -> key actions -> completion point]</user_flow_and_interactions>
<friction_reduction_notes>[How this sketch reduces friction/pain points]</friction_reduction_notes>
<variations>[Alternative design directions or variants]</variations>
</sketch>
[Repeat `<sketch>` for each sketch; total 3-5 sketches]
</sketch_descriptions>

FAILURE
- Root tag `<sketch_descriptions>` or child `<sketch>` sections are missing, malformed, or incomplete.
- Fewer than 3 or more than 5 sketches are provided.
- Any sketch is missing one or more required fields from `FORMAT`.
- Sketches are redundant and do not represent distinct flows/aspects.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
