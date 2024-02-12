---
title: Structured interview notes from transcript using flexible frameworks
category: User Research
tags:
  - user-research
  - interviews
  - transcripts
---
INPUTS
<provided_inputs>
- `{{INTERVIEW_TRANSCRIPT}}`: Source interview transcript.
- `{{NOTE_TAKING_MODE}}`: One of `Chronological`, `Topical`, `AEIOU Framework`, `Empathy Map`.
</provided_inputs>

GOAL
Convert interview transcripts into concise, evidence-grounded structured notes using a selected note-taking framework.
Success metric:
- Notes are concise, atomic, and traceable to transcript content.
- Organization strictly follows the selected note-taking mode.
- Output uses the required tagged structure and one-column table format.

CONSTRAINTS
- Use only provided inputs; if data is unclear, include explicit assumptions inside `<notes>` under an `Assumptions` subsection.
- Output only final notes wrapped in `<notes>` tags.
- Every note must:
- Capture exactly one idea.
- Be under 250 characters.
- Be grounded in transcript evidence.
- Use one-column markdown tables with clear category headers.
- Apply mode-specific organization:
- `Chronological`: single table ordered by transcript sequence.
- `Topical`: separate tables by major themes.
- `AEIOU Framework`: exactly five tables: Activities, Environments, Interactions, Objects, Users.
- `Empathy Map`: exactly eight tables: Thinks, Feels, Says, Does, Sees, Hears, Pains, Goals.
- If `{{NOTE_TAKING_MODE}}` is invalid or missing, default to `Topical` and record this in `Assumptions`.

FORMAT
Return exactly this structure:

<notes>
[Mode label]

[Category Header]
| Note |
| --- |
| [One atomic note under 250 chars] |
| [One atomic note under 250 chars] |

[Repeat tables according to selected mode]

Assumptions (only if needed)
| Note |
| --- |
| [Explicit assumption due to missing/ambiguous data] |
</notes>

FAILURE
- `<notes>` wrapper is missing or malformed.
- Tables are missing, not one-column, unlabeled, or not aligned with selected/default mode.
- Required mode categories are missing (AEIOU or Empathy Map).
- Notes exceed 250 characters, combine multiple ideas, or are not transcript-grounded.
- Output includes analysis/explanations outside structured notes.
- Assumptions are needed but not explicitly listed.
