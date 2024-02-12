---
title: "Multiple interface descriptions from a single image"
category: "Design & Prototyping"
tags:
  - pm
  - ux
  - design
  - communication
  - perspectives
---
INPUTS
<provided_inputs>
- {{IMAGE}}
</provided_inputs>

GOAL
Produce a high-quality deliverable for: "Multiple interface descriptions from a single image".
Success metric:
- Completes all required tasks and decision logic from the prompt instructions.
- Output is specific, evidence-based, and actionable.
- Output follows the required structure exactly.

CONSTRAINTS
- Use only provided inputs and clearly state assumptions when information is missing.
- Do not skip required analysis steps, sections, or validation logic.
- Keep recommendations/outputs grounded in the input context; avoid generic filler.
- Follow these task requirements:
<task_requirements>
You will be given an image of the interface for a complex tool. Your task is to describe this interface in four different ways. Here's how to proceed:

First, examine the image carefully:
<image>
{{IMAGE}}
</image>

Now, follow these steps:

1. Write instructions for a novice:  
   Analyze the image and write clear, step-by-step instructions for a beginner to understand and use the interface. Use simple language and explain each element of the interface. Begin your response with `<novice_instructions>` and end with `</novice_instructions>`.

2. Create a process diagram:  
   Based on your analysis of the image, create a textual representation of a process diagram. Use symbols like `[ ]` for steps, `( )` for decisions, and `->` for connections. Describe the flow of using the interface in a logical order. Begin your response with `<process_diagram>` and end with `</process_diagram>`.

3. Write like a 5th grader doing a book report:  
   Imagine you're a 5th grader writing a book report about this interface. Use simple vocabulary, short sentences, and an excited tone. Describe what you see and what you think it does. Begin your response with `<fifth_grader_report>` and end with `</fifth_grader_report>`.

4. Write for someone terminally online:  
   Rewrite your description for someone who spends all their time on the internet. Use internet slang, memes, and references. Be informal and use exaggerated language. Begin your response with ``.

Remember to base all your descriptions on the image provided. Do not invent features or elements that are not visible in the image. If you're unsure about any aspect of the interface, it's okay to say so in your descriptions.
</task_requirements>

FORMAT
Return exactly this structure:

<online_description>` and end with `</online_description>

FAILURE
- Output misses required sections, steps, or reasoning required by `<task_requirements>`.
- Required format/schema is missing, malformed, or incomplete.
- Claims are generic or not grounded in provided inputs.
- Assumptions are used but not explicitly stated.
