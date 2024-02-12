---
title: Positioning statements from competitive analysis and value proposition
category: Product Strategy
tags:
  - marketing
  - positioning
  - messaging
  - competitive-analysis
  - copywriting
---
INPUTS
<provided_inputs>
- {{TARGET_CUSTOMER}}
- {{UNMET_NEEDS}}
- {{PRODUCT_NAME}}
- {{PRODUCT_CATEGORY}}
- {{BENEFITS}}
- {{COMPETITIVE_LANDSCAPE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Positioning statements from competitive analysis and value proposition.
Success metric:
- Produces a canonical positioning statement plus two variants with clear differentiation.
- Uses outcomes over features, avoids buzzwords, and stays within length limits.
- Includes evidence hook and footnote for assumptions/prioritization when needed.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only the provided inputs; if any are missing or vague, infer minimally and wrap inferred text in [brackets].
- Output must be a single Markdown code block and nothing else.
- Include exactly one canonical statement and two variants (Executive-readout, Sales enablement).
- Enforce length limits: canonical <= 60 words; variants <= 35 words each.
- Avoid hype/buzzwords (for example: revolutionary, cutting-edge).
- Include an evidence hook in Differentiation without fabricating data.
- If multiple segments/competitors are provided, choose one and note in a footnote.

FORMAT
Return exactly this structure:

```markdown
## Positioning Statement

**For** [TARGET_CUSTOMER]  
**who** [UNMET_NEEDS in one tight clause],  
**[PRODUCT NAME]** **is a** [PRODUCT_CATEGORY]  
**that** [BENEFITS as results the user achieves].

### Differentiation
**Unlike** [PRIMARY COMPETITOR / STATUS QUO], **[PRODUCT NAME]** **delivers** [outcome-focused differentiation + proof hook].

---

## Executive-Readout Variant
For [TARGET_CUSTOMER], **[PRODUCT NAME]** is a [PRODUCT_CATEGORY] that [top outcome]. Unlike [competitor/status quo], it [sharp differentiator].

## Sales Enablement Variant
When [TARGET_CUSTOMER] struggles with [UNMET_NEEDS], **[PRODUCT NAME]** helps them [BENEFITS]. Unlike [competitor/alternative], it [differentiator tied to buying criteria].

[Optional Footnote: one sentence noting assumptions or prioritization choices]
```

FAILURE
- Output is not a single Markdown code block.
- Canonical or variant statements exceed length limits.
- Differentiation lacks an evidence hook.
- Missing or incorrect sections/labels from the required format.
- Footnote is missing when assumptions or prioritization are made.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
