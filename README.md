# Python-Screening-Task-2-Prompt-for-an-AI-Debugging-Assistant
Submission for Python Screening Task 2 – AI Debugging Assistant Prompt


This repository contains my submission for **FOSSEE Internship – Python Screening Task 2**.  
The task was to write a **natural-language prompt** for an AI debugging assistant that can help students identify and fix errors in their Python code **without directly giving the solution**.  



prompt--
You are an empathetic Python debugger supporting a student. Your task is to thoroughly examine the student's code, identify potential points of errors, and clarify them in easy-to-understand terms. Avoid providing the corrected code or complete solution. Instead, point out particular lines or reasoning that could be the issue, indicate what topic the student should look up, and provide hints or questioning guidance that lead the student to reflect critically on how to correct the bug. Always ensure your feedback is positive, concise, and learning-focused instead of simply fix-focused.

A brief explanation of your design choices---

1.Why you worded it the way you did:
-I combined a small organized output  with overt limits to ensure the assistant is both reliable and replicable for numerous problem types. The organization necessitates hard evidence-first diagnosis (line cites) followed by pedagogical scaffolding (progressive hints), which scales automation with instruction.

2.How you ensured it avoids giving the solution:
-(1) overt hard constraints preventing corrected code and exposing pseudocode; (2) incremental hinting — two hints and a micro-task only before demanding student action. (3) the assistant has to request the student to try the micro-task prior to providing more detailed assistance. Collectively these diminish the likelihood of the assistant providing a solution.

3.How it encourages helpful, student-friendly feedback:
-The prompt requires supportive language, evidence-based classification, and open-ended questions that prod thinking instead of doing. Micro-tasks make debugging feasible but also need the student to do the work. The "confidence" tag indicates doubt and encourages student verification.

Reasoning---

1.What tone and style should the AI use when responding?
-Supportive, patient, and Socratic. Brief sentences, plain language, celebrate what's right first, and keep it brief. Resort to questions and prods instead of orders.

2.How should the AI balance between identifying bugs and guiding the student?
-Prioritize recognition with explicit proof. Following diagnosis, transition into guidance through questions and micro-tasks that enable the student to try out hypotheses. Save particular, directed cues only after the student has attempted something or requested additional assistance (progressive disclosure). 

3.How would you adapt this prompt for beginner vs. advanced learners?
-Novice adaptation:
Adopt simpler terminology and add an additional Hint Level that gives a narrowly defined definition of the applicable concept (still no fix).
Example tweak line: "Use simple, concrete terminology; when referring to concepts, add an accompanying one-sentence mini-definition.

-Advanced adaptation:
Be shorter, skip definition of basic concepts, and center hints around invariants, edge cases, complexity, or design intent. Let the assistant provide targeted test suggestions and request the student's mental model of the algorithm.

Setup Instructions--

1. Replicate the prompt from the "Prompt" section above.
2. Copy it and paste it in an AI tool like ChatGPT.
3. Include an example of buggy Python code to execute.
4. See how the AI replies with hints and explanations "without giving out the full corrected solution".

Submission Checklist---

-  Prompt is clear, specific, and well-structured  
-  Reasoning is thoughtful and well-articulated  
-  Includes reasoning answers

  

Author  
Shreena Mani  


