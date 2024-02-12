---
title: PRDs from industry and feature specifications
category: Business Analysis
tags:
  - pm
  - prd
  - requirements
  - documentation
  - business-analysis
---
INPUTS
<provided_inputs>
- {{INDUSTRY}}
- {{COMPANY_NAME}}
- {{FEATURE_NAME}}
- {{DEVELOPMENT_STAGE}}
- {{CURRENT_KNOWLEDGE}}
- {{CURRENT_SOLUTION}}
</provided_inputs>

GOAL
Create a complete, implementation-ready PRD for `FEATURE_NAME` in the specified `INDUSTRY` and `DEVELOPMENT_STAGE`.
Success metric:
- Covers all required PRD sections with actionable detail.
- Aligns recommendations to current stage, known constraints, and existing solution context.
- Uses explicit assumptions where information is missing.
- Follows the required output structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip any required PRD section.
- Ground requirements in `CURRENT_KNOWLEDGE` and `CURRENT_SOLUTION`; do not contradict provided context without explicit rationale.
- Use the exact PRD heading/table structure specified in `FORMAT`.
- Keep requirements testable and implementation-oriented where possible.
- Maintain a professional, industry-appropriate tone.

FORMAT
Return exactly this structure:

<PRD>
# [Product Name]

## About
[High-level overview of the product and goal.]

## Market Insights
[Market context, competitors, trends, and target users.]

## Problem
[Core user problem, pain points, and why existing solutions are insufficient.]

## Solution
[Proposed AI product solution and how it addresses the problem.]

## Feature Prioritization
| Feature | Reach | Impact | Confidence | Effort | RICE Score | Priority |
|---------|-------|--------|------------|--------|------------|----------|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Requirements
**Functional Requirements:**
- FR1:
- FR2:
- FR3:

**AI/ML Model Requirements:**
- MR1:
- MR2:
- MR3:

**Non-Functional Requirements:**
- NFR1:
- NFR2:
- NFR3:

## Challenges
[Key product, technical, data, and go-to-market challenges.]

## Positioning
| Use Case | Target User | Key Benefit | Differentiator |
|----------|-------------|-------------|----------------|
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

## Metrics
[Success metrics and north star metric.]

## Rollout Plan
- **Stakeholders & Communication**
  - [Stakeholder groups and communication plan]

- **Roll-out Strategy**
  - [Launch phases, gating criteria, and post-GA plan]
</PRD>

FAILURE
- Any required section/table/list item pattern from `FORMAT` is missing or materially incomplete.
- Content is generic and not grounded in provided inputs.
- Requirements are not actionable/testable.
- Development-stage alignment is missing.
- Required output schema is missing or malformed.
