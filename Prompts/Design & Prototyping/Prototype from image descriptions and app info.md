---
title: Prototype creation from image descriptions and app info
category: Design & Prototyping
tags:
  - pm
  - ux
  - prototyping
  - html
  - interaction-design
---
INPUTS
<provided_inputs>
- {{IMAGE_DESCRIPTION}}
- {{APP_INFO}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Prototype creation from image descriptions and app info.
Success metric:
- Produces a coherent clickable screen prototype aligned with provided image/app context.
- Includes complete HTML, CSS, and JavaScript with responsive layout and interactive behavior.
- Returns incremental build artifacts plus a final merged prototype file.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{IMAGE_DESCRIPTION}}` and `{{APP_INFO}}`; if details are missing, state assumptions explicitly.
- Build a realistic screen mental model before coding.
- Provide incremental artifacts in this order:
  - `html_structure`
  - `css_styles`
  - `js_functionality`
  - `final_prototype`
- `html_structure` must include `<!DOCTYPE html>`, `<html>`, `<head>`, `<title>`, and `<body>` scaffolding.
- `css_styles` must include responsive layout rules and clear interactive states.
- `js_functionality` must implement click behavior for primary interactive elements.
- `final_prototype` must combine valid HTML+CSS+JS into one executable file snippet.
- Keep the prototype suitable for user testing: functional, readable, and context-aligned.

FORMAT
Return exactly this structure:

<html_structure>
[Basic HTML scaffold only]
</html_structure>

<css_styles>
[CSS for layout, components, states, and responsiveness]
</css_styles>

<js_functionality>
[JavaScript for interactions, click handlers, and lightweight transitions]
</js_functionality>

<final_prototype>
[Single complete HTML file containing merged HTML, CSS, and JS]
</final_prototype>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, out of order, or incomplete.
- `final_prototype` does not contain a full standalone HTML document.
- Interactive elements are described but not implemented in JavaScript.
- Layout is not responsive or lacks interaction feedback states.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
