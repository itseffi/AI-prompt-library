---
title: Product feature impact sizing from metrics and usage data
category: Business Analysis
tags:
  - pm
  - business-analysis
  - impact-sizing
  - metrics
  - analytics
---
INPUTS
<provided_inputs>
- {{PRODUCT_FEATURE}}
- {{METRICS}}
</provided_inputs>

GOAL
Estimate the potential impact of `PRODUCT_FEATURE` using `METRICS` with transparent assumptions, calculations, and sensitivity ranges.
Success metric:
- Builds a usage funnel from exposure to actual usage.
- Quantifies engagement, top-line, and bottom-line effects with explicit math.
- Identifies weakest assumptions and proposes de-risk actions plus scenarios.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis stages:
  1. Usage funnel estimation (exposed -> activated -> used).
  2. Impact quantification (engagement, top-line, bottom-line).
  3. Risk/assumption analysis (weakest assumptions, de-risk methods, scenarios).
  4. Strategic takeaways and recommendations.
- Show formulas and intermediate calculations; avoid unsupported point estimates.
- Include assumptions next to each major calculation.
- Keep outputs concrete and grounded in provided metrics/context.

FORMAT
Return exactly this structure:

<analysis>
<introduction>[Brief role/task framing]</introduction>
<usage_funnel>[Exposure-to-usage funnel with assumptions and drop-off reasoning]</usage_funnel>
<impact_calculations>
<engagement>[DAU/MAU/retention impact estimates with formulas]</engagement>
<top_line>[GMV/revenue impact estimates with formulas]</top_line>
<bottom_line>[Contribution margin/net income impact estimates with formulas]</bottom_line>
</impact_calculations>
<assumption_risk_and_scenarios>[Riskiest assumptions, de-risk plan, conservative/base/aggressive scenarios]</assumption_risk_and_scenarios>
<takeaways>[Implications for planning, experimentation, and feature design]</takeaways>
</analysis>

FAILURE
- Any required section in `FORMAT` is missing or malformed.
- Impact estimates are provided without formulas/intermediate reasoning.
- Usage funnel is missing or does not connect exposure to actual usage.
- No sensitivity scenarios or no de-risk actions for weak assumptions.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
