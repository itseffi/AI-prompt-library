---
title: "Offbeat question generation from any topic"
category: "Ideation & Creativity"
tags:
  - creativity
  - brainstorming
  - questions
  - perspective-shifting
---
INPUTS
<provided_inputs>
- {{TOPIC}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Offbeat question generation from any topic".
Success metric:
- Produces playful, imaginative, and topic-relevant offbeat questions.
- Includes at least 3 offbeat "why" questions and at least 2 offbeat questions in other forms.
- Questions show variety (comparisons, hypotheticals, absurd twists) rather than minor rewrites.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{TOPIC}}`; if topic scope is ambiguous, state assumptions explicitly.
- Generate at least 3 offbeat `why` questions tied to the topic.
- Generate at least 2 additional offbeat questions in non-`why` formats (for example: `what if`, `how come`, or other playful forms).
- Keep questions imaginative and thought-provoking while staying topic-relevant.
- Avoid repetitive templates and near-duplicate wording.

FORMAT
Return exactly this structure:

<offbeat_questions>
<why_questions>
1. [Your first "why" question]
2. [Your second "why" question]
3. [Your third "why" question]
[Add more if you generate more than 3]
</why_questions>

<other_questions>
1. [Your first other offbeat question]
2. [Your second other offbeat question]
[Add more if you generate more than 2]
</other_questions>
</offbeat_questions>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Fewer than 3 `why` questions are provided.
- Fewer than 2 `other_questions` are provided.
- `other_questions` are all `why` questions.
- Questions are repetitive or generic with no clear offbeat angle.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
