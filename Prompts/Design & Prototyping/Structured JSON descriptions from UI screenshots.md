---
title: "Structured JSON descriptions from UI screenshots"
category: "Design & Prototyping"
tags:
  - pm
  - ux
  - design
  - ui
  - json
---
INPUTS
<provided_inputs>
- {{SCREENSHOT}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Structured JSON descriptions from UI screenshots".
Success metric:
- Produces a detailed, structured JSON description of the UI screenshot.
- Captures layout, visual style, text, UI elements, imagery/icons, and hierarchy with high fidelity.
- Flags ambiguities explicitly without inventing unsupported details.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{SCREENSHOT}}`; if details are unclear, state uncertainty in `notes`.
- Do not invent hidden functionality or off-screen content.
- Capture:
  - overall layout and structure,
  - color scheme,
  - UI elements (interactive and non-interactive),
  - text content,
  - images/icons,
  - hierarchy/positioning.
- For each `ui_elements` item include `type`, `content`, `position`, and `style`.
- Keep output as valid JSON only inside `<json_output>` tags (no prose outside JSON).

FORMAT
Return exactly this structure:

<json_output>
{
  "overall_layout": {
    "description": "",
    "main_sections": []
  },
  "color_scheme": {
    "primary_colors": [],
    "secondary_colors": [],
    "background_color": ""
  },
  "ui_elements": [
    {
      "type": "",
      "content": "",
      "position": "",
      "style": {}
    }
  ],
  "text_content": [
    {
      "type": "",
      "content": "",
      "position": ""
    }
  ],
  "images_and_icons": [
    {
      "type": "",
      "description": "",
      "position": ""
    }
  ],
  "notes": []
}
</json_output>

FAILURE
- Output is not wrapped in `<json_output>` tags.
- JSON is invalid or required top-level keys are missing.
- `ui_elements` entries are missing `type`, `content`, `position`, or `style`.
- Observations are generic and not grounded in visible screenshot evidence.
- Ambiguities exist but `notes` is omitted.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
