# Skill Formation Paper Summary

Paper: "How AI Impacts Skill Formation" (Judy Hanwen Shen & Alex Tamkin, Anthropic Fellows Program).

## Most Important Findings

1. AI assistance hurt skill formation, with no clear speed gain.
In a randomized experiment, developers learned a new async Python library (Trio) with or without an AI assistant. The AI group scored ~17% lower on a comprehension quiz (about 2 grade points, Cohen's d = 0.738, p = 0.01), and did not complete the task significantly faster on average.

2. The biggest losses were exactly the skills needed to supervise AI.
AI users were worse at conceptual understanding, code reading, and especially debugging, the largest gap. These are the abilities required to catch and fix wrong AI-generated code.

3. Struggling with errors is where learning happens.
The control group (no AI) hit far more errors (median 3 vs 1), including library-specific ones. Encountering and independently resolving these errors is what built real understanding. AI smoothed over the errors and the learning with them.

4. How you use AI matters more than whether you use it.
The authors identified six interaction patterns, split into low- and high-scoring:
- Low-scoring (~24-39%): full delegation, progressive reliance, iterative AI debugging. Heavy code generation, little independent thinking.
- High-scoring (~65-86%): conceptual questions only, code + explanation, generate-then-comprehend. More cognitive effort, AI used to deepen understanding.

5. Cognitive effort, not time, drives learning.
Manually typing AI code vs pasting it made no difference to quiz scores. What separated high scorers was active engagement (asking why, seeking explanations), not how long they spent.

6. "Productivity" can be an illusion that hides cost.
Only ~20% of AI users (full delegators) were actually faster. AI users found the task easier and reported feeling "lazy" with "gaps in understanding," while the no-AI group reported more learning and enjoyment.

7. Implication for safety-critical work.
As teams shift to AI writing code with human supervision, workers whose own skills were eroded by AI may be unable to validate or debug what the AI produced. AI-enhanced productivity is "not a shortcut to competence."

## 3 Questions for an Interactive Session (Software Teams)

1. Where are we using AI to finish work versus to understand it?
On recent tasks, did we ask AI to just generate the solution, or did we ask it to explain concepts so we'd learn? Which pattern is our default?

2. What skills are we quietly outsourcing, and would we notice if we lost them?
If AI couldn't help tomorrow, where would we struggle most: debugging, reading unfamiliar code, understanding a new library? That gap is our real exposure.

3. How do we keep "productive struggle" in our workflow?
The errors people fight through are where skill forms. For onboarding and new tools, where should we deliberately slow down and engage rather than let AI smooth the path?