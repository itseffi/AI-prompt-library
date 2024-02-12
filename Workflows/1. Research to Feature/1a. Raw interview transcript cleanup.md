---
title: Raw interview transcript cleanup
category: User Research
tags:
  - user-research
  - interviews
  - transcripts
---
INPUTS
<provided_inputs>
- `{{RAW_TRANSCRIPT}}`: Raw interview transcript with speaker turns.
</provided_inputs>

GOAL
Clean a raw interview transcript for readability while preserving original meaning, intent, and speaker voice.
Success metric:
- Transcript is easier to read and remains faithful to original content.
- Speaker labels and conversational flow are preserved.
- Output follows the required schema exactly.

CONSTRAINTS
- Use only the provided transcript content.
- Make light edits only; do not summarize, reinterpret, or remove meaningful content.
- Remove filler words, false starts, and redundant repetitions only when they do not change meaning.
- Preserve each speaker's voice and tone; avoid over-formalizing casual language.
- Keep original speaker labels at the beginning of each turn (for example: `Interviewer:`, `Interviewee:`).
- Preserve unclear/inaudible markers exactly as given (for example: `[inaudible]`).
- Correct punctuation and capitalization for readability.
- Do not add commentary, analysis, or extra sections.

FORMAT
Return exactly this structure:

<edited_transcript>
[Cleaned transcript text with original speaker labels and turn order preserved.]
</edited_transcript>

FAILURE
- Output is not wrapped in `<edited_transcript>` tags.
- Meaning, intent, or factual content is altered.
- Speaker labels are removed, changed, or inconsistently applied.
- Transcript is over-edited (excessive cuts, paraphrasing, or tone normalization).
- Inaudible/unclear markers from source are removed or rewritten.
- Extra sections, commentary, or metadata are included.
