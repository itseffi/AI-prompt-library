---
title: Acceptance criteria for UI
category: Technical
tags:
  - quality-assurance
  - ui
  - acceptance-criteria
  - responsive-design
  - technical
---
INPUTS
<provided_inputs>
- [No explicit variables declared; use provided context.]
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Acceptance criteria for UI.
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Produce a testable UI acceptance-criteria and QA validation checklist for the provided UI context.
- Cover at minimum:
- Visual testing (default/state/responsive checks).
- Functional testing (primary action, loading, error handling, edge cases).
- Accessibility testing (keyboard, screen reader, contrast, ARIA/semantic checks).
- Browser/device compatibility.
- Pass/fail summary with issues, tester, and date.
- Keep checks specific and verifiable (observable behavior, measurable thresholds, concrete expected results).
- Use a checklist style suitable for QA execution.

FORMAT
Return exactly this structure:

<qa_validation>
## QA Validation Checklist

### Visual Testing
- [ ] [check]
- [ ] [check]

### Functional Testing
- [ ] [check]
- [ ] [check]

### Accessibility Testing
- [ ] [check]
- [ ] [check]

### Browser Compatibility
- [ ] Chrome (latest): [result]
- [ ] Safari (latest): [result]
- [ ] Firefox (latest): [result]
- [ ] Edge (latest): [result]
- [ ] Safari iOS: [result]
- [ ] Chrome Android: [result]

### Pass/Fail
**Overall Result:** [PASS or FAIL]
**Issues Found:** [list deviations or "None"]
**Tester:** [name]
**Date:** [date]
</qa_validation>

FAILURE
- `<qa_validation>` schema is missing, malformed, or materially incomplete.
- Checklist items are vague/non-testable (no clear expected behavior or measurable criteria).
- Any critical section (Visual, Functional, Accessibility, Browser Compatibility, Pass/Fail) is missing.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
