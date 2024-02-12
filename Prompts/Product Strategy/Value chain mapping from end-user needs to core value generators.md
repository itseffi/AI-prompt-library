---
title: Value chain mapping from end-user needs to core value generators
category: Product Strategy
tags:
  - strategy
  - value-chain
  - business-model
  - structured-thinking
---
INPUTS
<provided_inputs>
- {{PRODUCT}}
- {{INDUSTRY}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: Value chain mapping from end-user needs to core value generators.
Success metric:
- Maps end-user needs to a full value chain and identifies core value generators.
- Highlights vulnerabilities where the chain could be disrupted.
- Grounds analysis in the provided product and industry context.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only `{{PRODUCT}}` and `{{INDUSTRY}}`; if information is missing, state assumptions explicitly.
- Map value creation from end-user needs back to foundational inputs.
- Identify core value generators and explain why they are defensible.
- Highlight vulnerabilities and potential disruption points.
- Keep analysis specific to the product/industry context.

FORMAT
Return exactly this structure:

<value_chain_analysis>
1. End-user needs:  
   [List the primary needs the product/service fulfills]

2. Value chain breakdown:  
   [Provide a hierarchical breakdown of the value chain, from end-user needs to basic inputs]

3. Core value generators:  
   [List and explain the identified core value generators]

4. Potential vulnerabilities:  
   [Discuss any aspects of the value chain that could be vulnerable to disruption]
</value_chain_analysis>

FAILURE
- Any required section/tag in `FORMAT` is missing, malformed, or incomplete.
- Value chain breakdown does not reach foundational inputs.
- Core value generators lack defensible rationale.
- Vulnerabilities are missing or generic.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
