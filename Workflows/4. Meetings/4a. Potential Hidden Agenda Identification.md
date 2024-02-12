---
title: Potential Hidden Agenda Identification
category: Stakeholder Management
tags:
  - stakeholders
  - analysis
  - organizational-politics
  - negotiation
  - stakeholder-management
---
INPUTS
<provided_inputs>
- {{SITUATION_DESCRIPTION}}
- {{STAKEHOLDERS_LIST}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Potential Hidden Agenda Identification.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Analyze `{{SITUATION_DESCRIPTION}}` and `{{STAKEHOLDERS_LIST}}` to identify plausible hidden agendas per stakeholder.
- For each stakeholder, assess official stance, personal/professional incentives, historical behavior (if provided), relationships, and outcome-based benefits/risks.
- Use objective, evidence-based reasoning and reasonable inferences only; avoid unsupported speculation.
- Consider multiple agenda possibilities where uncertainty exists.
- Include a brief overall summary describing interactions/conflicts among stakeholder agendas.

FORMAT
Return exactly this structure:

<stakeholder_analysis>
   <stakeholder_name>[Name of the stakeholder]</stakeholder_name>
   <official_position>[Brief description of their official stance or role]</official_position>
   <potential_hidden_agenda>[Your analysis of their possible hidden agenda]</potential_hidden_agenda>
   <supporting_factors>[List key factors that support your analysis]</supporting_factors>
</stakeholder_analysis>
[Repeat `<stakeholder_analysis>` for each stakeholder in `{{STAKEHOLDERS_LIST}}`]

<overall_summary>
[Brief summary of how potential hidden agendas interact, align, or conflict across stakeholders]
</overall_summary>

FAILURE
- Any stakeholder is missing a `<stakeholder_analysis>` block or required child tags.
- `<overall_summary>` is missing or does not address interactions/conflicts between agendas.
- Analysis is speculative, biased, or not grounded in provided information.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
