---
title: Conversation summaries from meeting transcripts
category: Project Management
tags:
  - meetings
  - summarization
  - note-taking
  - communication
---
INPUTS
<provided_inputs>
- {{CONVERSATION}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Conversation summaries from meeting transcripts.
Success metric:
- Produces a structured summary of major topics with correct hierarchy.
- Extracts explicit actions with owners and ADHD-friendly step breakdowns.
- Keeps summary faithful to the transcript without fabrication.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{CONVERSATION}}`; if information is missing, state assumptions explicitly.
- Summarize with nested bullets reflecting topic hierarchy and relationships.
- Identify explicit actions with:
  - `**Action:**` statement,
  - `**Who:**` owner,
  - concise numbered ADHD-friendly steps.
- Keep language clear and concise; avoid invented facts or inferred decisions not in transcript.
- Output must be inside `<summary>` tags only.

FORMAT
Return exactly this structure:

<summary>
• Main topic 1
  ◦ Subtopic 1.1
    ▪ Detail 1.1.1
    ▪ Detail 1.1.2
  ◦ Subtopic 1.2
    ▪ Detail 1.2.1
      - Sub-detail 1.2.1.1

• Main topic 2
  ◦ Subtopic 2.1
    ▪ **Action: [Description of the action]**
    ▪ **Who: [Person responsible]**
    ▪ Steps for ADHD individuals:
      1. First step
      2. Second step
      3. Third step

  ◦ Subtopic 2.2
    ▪ Detail 2.2.1
</summary>

FAILURE
- `<summary>` wrapper is missing, malformed, or incomplete.
- Nested structure does not reflect major topics and supporting details.
- Actions are missing `**Action:**`, `**Who:**`, or ADHD step breakdown.
- Content includes fabricated points not present in transcript.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
