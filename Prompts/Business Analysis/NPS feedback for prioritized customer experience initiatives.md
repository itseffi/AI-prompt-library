---
title: NPS feedback for prioritized customer experience initiatives
category: Business Analysis
tags:
  - pm
  - business-analysis
  - nps
  - customer-experience
  - prioritization
---
INPUTS
<provided_inputs>
- {{NPS_FEEDBACK}}
</provided_inputs>

GOAL
Translate `NPS_FEEDBACK` into a prioritized initiative backlog that reduces detractor pain and amplifies promoter value.
Success metric:
- Separates detractors (0-6) and promoters (9-10) correctly.
- Identifies top recurring themes with evidence (frequency + representative quote).
- Produces prioritized initiatives with transparent scoring and clear ownership-ready descriptions.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Treat only scores `0-6` as detractors and `9-10` as promoters; ignore or label neutral scores (`7-8`) if present.
- Identify top 5 detractor pain themes and top 5 promoter benefit themes from recurring signals.
- For each theme, include:
  - short theme label,
  - brief description,
  - frequency signal (count or relative frequency),
  - at least one representative quote.
- For each proposed initiative, provide a `Priority Score` from `1-5` based on:
  - Frequency (how often theme appears),
  - Impact (customer experience importance),
  - Feasibility (implementation realism).
- Keep initiatives concrete and implementation-ready (avoid generic statements).

FORMAT
Return exactly this structure:

<output>
<theme_analysis>
<detractor_themes>
1. [Theme]
   - Description: [Brief description]
   - Frequency: [Count or relative frequency]
   - Representative Quote: "[Quote]"
[Repeat to top 5]
</detractor_themes>
<promoter_themes>
1. [Theme]
   - Description: [Brief description]
   - Frequency: [Count or relative frequency]
   - Representative Quote: "[Quote]"
[Repeat to top 5]
</promoter_themes>
</theme_analysis>

<detractor_initiatives>
1. [Initiative Name] (Priority Score: X)  
   - Description: [Brief description of the initiative]  
   - Addresses: [Pain point being addressed]  
   - Scoring Rationale: [Frequency / Impact / Feasibility rationale]
   - Representative Quote: "[Direct quote from feedback]"

[Repeat for top 3-5 detractor initiatives]
</detractor_initiatives>

<promoter_initiatives>
1. [Initiative Name] (Priority Score: X)  
   - Description: [Brief description of the initiative]  
   - Amplifies: [Benefit being amplified]  
   - Scoring Rationale: [Frequency / Impact / Feasibility rationale]
   - Representative Quote: "[Direct quote from feedback]"

[Repeat for top 3-5 promoter initiatives]
</promoter_initiatives>

<summary>
[Provide a brief summary of the key findings and the potential impact of implementing these initiatives]
</summary>
</output>

FAILURE
- Detractor/promoter segmentation is incorrect or not shown.
- Theme analysis is missing top recurring themes, frequencies, or quotes.
- Initiatives are missing priority scores or scoring rationale.
- Recommendations are generic or not linked to identified themes.
- Required schema is missing, malformed, or incomplete.
- Assumptions are used but not explicitly stated.
