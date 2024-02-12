---
title: Problem framing before jumping to solutions
category: User Research
tags:
  - user-research
  - problem-framing
  - product-design
---
INPUTS
<provided_inputs>
- `{{PROPOSED_SOLUTION}}`: The proposed solution idea or concept.
- `{{CONTEXT}}`: Product, user, business, and operational context related to the proposal.
</provided_inputs>

GOAL
Reorient teams from premature solution mode to rigorous, evidence-driven problem framing before solution design.
Success metric:
- The analysis diagnoses solution-jumping clearly and identifies assumptions, evidence, and risks.
- The output defines a user-centered problem statement with measurable success criteria.
- The output provides a concrete validation research plan and preserves collaborative team alignment.

CONSTRAINTS
- Use only provided inputs; if information is missing, state explicit assumptions.
- Diagnose the proposed solution before prescribing alternatives.
- Address all required analysis steps:
- Identify solution-jumping (proposed solution, embedded assumptions, implied problem, evidence status).
- Extract underlying problem (user need, JTBD, desired outcome, current state, constraints).
- Challenge assumptions (validity, evidence, risk if wrong, validation method).
- Frame a complete problem statement (who, where/when, impact, workarounds, success).
- Provide alternative problem framings to widen exploration.
- Propose pre-solution research to validate the problem.
- Recommendations must be specific, testable, and grounded in `{{CONTEXT}}`.
- Maintain a collaborative tone that frames validation as de-risking, not rejection.

FORMAT
Return exactly this structure:

<problem_framing_analysis>
<solution_jumping_diagnosis>
**Proposed Solution:**
[Describe the solution being discussed]

**Embedded Assumptions:**
[List assumptions built into this solution:
- Assumes users need X
- Assumes current problem is Y
- Assumes best approach is Z]

**Implied Problem:**
[What problem is this solution trying to solve?]

**Evidence Status:**
[What evidence exists that this is the right problem to solve? What's missing?]
</solution_jumping_diagnosis>

<underlying_problem_extraction>
**User Need:**
[What fundamental user need is being addressed?]

**Job-to-be-Done:**
[What job is the user trying to accomplish?]

**Desired Outcome:**
[What result does the user want to achieve?]

**Current State:**
[How do users accomplish this today? What goes wrong?]

**Constraints:**
[What limitations exist: technical, business, user, environmental?]
</underlying_problem_extraction>

<assumption_challenges>
[For each key assumption, ask:
- Assumption: [state it]
- Is it validated? [Yes/No/Partially]
- Evidence: [what supports or contradicts it]
- Risk if wrong: [what happens if this assumption is false]
- How to validate: [proposed test]]
</assumption_challenges>

<problem_statement>
**Who:** [Specific user segment]

**Experiences:** [Specific problem or friction]

**When/Where:** [Context and triggers]

**Impact:** [Consequence and severity]

**Current Workarounds:** [What users do today]

**Success Would Be:** [Measurable outcome]

**Problem Statement:**
[Complete: "Users [who] struggle to [what] when [context] because [root cause], which leads to [impact]. Success would mean [outcome]"]
</problem_statement>

<alternative_problem_framings>
<framing_1>
[Present alternative way to frame this problem that might lead to different solutions]
</framing_1>

<framing_2>
[Present second alternative framing]
</framing_2>

<framing_3>
[Present third alternative framing if applicable]
</framing_3>
</alternative_problem_framings>

<validation_research>
**Research Questions:**
[List 5-7 questions that would validate the problem:
- Do users actually experience this problem?
- How frequently and severely?
- What triggers it?
- How do they currently cope?
- What would "solved" look like to them?]

**Proposed Method:**
[Suggest appropriate research approach:
- User interviews focused on problem space
- Observational research of current workflows
- Diary studies to capture problem in context
- Analytics analysis of behavior patterns]

**Success Criteria:**
[What would confirm this is the right problem to solve?]

**Timeline:**
[How long would this research take?]
</validation_research>

<solution_divergence_plan>
**Once Problem Is Validated:**

**Divergence Questions:**
[Questions to open up solution space:
- How might we [solve aspect 1]?
- What if [constraint] didn't exist?
- How do other domains solve similar problems?
- What would the ideal solution look like?]

**Solution Criteria:**
[What should any solution achieve? List must-haves and nice-to-haves]

**Exploration Approach:**
[Suggest how to explore solutions once problem is understood:
- Competitive analysis
- Analogous research
- Design studio
- Rapid prototyping]
</solution_divergence_plan>

<communication_strategy>
**How to Redirect the Team:**
[Suggest how to shift the conversation from solution to problem:
- Acknowledge the solution thinking
- Reframe as problem exploration
- Show value of problem validation
- Set timeline for problem then solution phases]

**Draft Message:**
[Provide a tactful message to the team explaining the value of problem framing]
</communication_strategy>
</problem_framing_analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, reordered, or materially incomplete.
- Analysis skips core problem-framing steps (solution-jumping diagnosis, problem extraction, assumption challenge, validation plan).
- Claims are generic, not evidence-linked, or not grounded in provided inputs.
- Output proposes solutions before adequately framing/validating the problem.
- Assumptions or uncertainties are used but not explicitly stated.
- Tone is adversarial or dismissive rather than collaborative and de-risking.
