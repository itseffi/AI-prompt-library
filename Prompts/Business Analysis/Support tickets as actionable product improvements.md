---
title: Support tickets as actionable product improvements
category: Business Analysis
tags:
  - pm
  - business-analysis
  - support
  - product-improvements
  - feedback
---
INPUTS
<provided_inputs>
- {{SUPPORT_TICKETS}}
</provided_inputs>

GOAL
Convert `SUPPORT_TICKETS` into evidence-backed trends and a prioritized product-improvement backlog.
Success metric:
- Categorizes ticket themes with clear frequency/severity signals.
- Identifies major recurring patterns and notable critical issues.
- Produces prioritized improvements tied to explicit ticket evidence.
- Follows the required output schema exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps:
  1. Categorize tickets/issues.
  2. Quantify category frequency.
  3. Identify recurring themes and severe/unusual issues.
  4. Detect pattern signals (cross-user, time-based, or correlated issues when available).
  5. Prioritize improvements by frequency, severity/impact, and estimated effort.
- Keep all claims grounded in provided support-ticket data.
- Label assumptions if timestamps, severity labels, or effort signals are missing.

FORMAT
Return exactly this structure:

<trend_analysis>
[3-5 major trends with evidence from support tickets, including category frequency and notable severe issues]
</trend_analysis>

<prioritized_improvements>
List at least 5 prioritized improvements, ranked from highest to lowest priority. For each improvement:
1. [Improvement Name]
   - Description: Brief description of the improvement
   - Justification: Explain why this improvement is important, citing specific trends or issues from the data
   - Priority Drivers: Frequency / Severity / Effort rationale
   - Potential Impact: Describe the expected positive impact on user experience
</prioritized_improvements>

FAILURE
- Missing `<trend_analysis>` or `<prioritized_improvements>`.
- Fewer than 5 prioritized improvements.
- Prioritization is not supported by frequency/severity/effort reasoning.
- Claims are generic or not grounded in provided ticket evidence.
- Assumptions are used but not explicitly stated.
