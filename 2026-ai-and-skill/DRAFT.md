# AI and Skill

1. Cognitive Debt

   1. **The term comes from an EEG study.** MIT Media Lab's "Your Brain on ChatGPT" (Kosmyna et al.) coined "cognitive debt" to describe the accumulated cognitive cost of relying on an LLM. Over 4 months, the LLM group consistently underperformed the brain-only group at the neural, linguistic, and behavioral levels. ([arXiv:2506.08872](https://arxiv.org/abs/2506.08872), [MIT Media Lab](https://www.media.mit.edu/projects/your-brain-on-chatgpt/overview/))

   2. **Brain connectivity scales down with tool support.** EEG showed brain-only writers had the strongest, most distributed neural networks; search-engine users moderate; LLM users the weakest coupling — measurable under-engagement of alpha and beta networks. ([arXiv:2506.08872](https://arxiv.org/abs/2506.08872))

   3. **Lower ownership and recall.** LLM users reported the lowest ownership of their own essays and struggled to quote work they had written minutes earlier — a sign that knowledge was never internalized. ([arXiv:2506.08872](https://arxiv.org/abs/2506.08872))

   4. **At team level, cognitive debt is the erosion of shared understanding.** Storey reframes it as a project-level property: no one can confidently explain how the system works or predict the impact of a change. GenAI can reduce technical debt while accelerating cognitive (and intent) debt. ([ACM Queue, "From Technical Debt to Cognitive and Intent Debt"](https://queue.acm.org/detail.cfm?id=3746117))

   5. **It is invisible until changes start failing.** Warning signals: resistance to change, surprising side effects from "simple" changes, slow onboarding despite docs, loss of who-knows-what (transactive memory), and low bus factor. Mitigation: treat understanding as a deliverable (walkthroughs, code review, retrospectives, intent-first workflows). ([ACM Queue](https://queue.acm.org/detail.cfm?id=3746117))

2. Cognitive Surrender

   1. **A "third system" of thinking.** Shaw & Nave (Wharton) extend Kahneman's dual-process model — System 1 (fast/intuitive), System 2 (slow/deliberate) — with **System 3**: external, AI-based cognition. Cognitive surrender is adopting System 3's output with minimal scrutiny, overriding both intuition and deliberation. ([Tri-System Theory, Shaw & Nave (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6097646))

   2. **Distinct from cognitive offloading.** Offloading is the strategic delegation of a discrete task to a tool (calculator, linter). Surrender is a deeper abdication of critical evaluation — the user relinquishes cognitive control and adopts the AI's judgment as their own. ([Shaw & Nave (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6097646), [ACM Queue, Storey](https://queue.acm.org/detail.cfm?id=3746117))

   3. **People follow AI even when it's wrong.** Across 3 preregistered experiments (N = 1,372; ~9,600 trials), participants consulted the AI on a majority of trials. Accuracy rose ~+25 points when the AI was correct and fell ~-15 points when it erred — the behavioral signature of surrender (Cohen's h = 0.81). ([Shaw & Nave (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6097646))

   4. **It inflates confidence, even after errors.** Engaging System 3 raised confidence even following wrong answers. People feel more sure while being less correct — which is why the resulting cognitive debt stays hidden until changes start failing. ([Shaw & Nave (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6097646))

   5. **Context and traits modulate it.** Time pressure increases surrender; per-item incentives plus immediate feedback reduce it (but don't eliminate it). Higher trust in AI → more surrender; higher need for cognition and fluid intelligence → more resistant. ([Shaw & Nave (SSRN)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6097646))

3. Skill formation

   1. **AI assistance hurt learning with no clear speed gain.** In a randomized experiment, developers learned a new async Python library (Trio) with or without AI. The AI group scored ~17% lower on a comprehension quiz (~2 grade points, Cohen's d = 0.738, p = 0.01) and were not significantly faster on average. ([Shen & Tamkin, "How AI Impacts Skill Formation" (arXiv)](https://arxiv.org/abs/2601.20245))

   2. **The biggest losses were the skills needed to supervise AI.** AI users were worse at conceptual understanding, code reading, and especially debugging — the largest gap. These are exactly the abilities required to catch and fix wrong AI-generated code. ([Shen & Tamkin (arXiv)](https://arxiv.org/abs/2601.20245))

   3. **Struggling with errors is where learning happens.** The no-AI group hit more errors (median 3 vs 1) and resolved them independently — building real understanding. AI smoothed over the errors, and the learning with them. ([Shen & Tamkin (arXiv)](https://arxiv.org/abs/2601.20245))

   4. **How you use AI matters more than whether you use it.** Six interaction patterns split into low-scoring (full delegation, progressive reliance, iterative AI debugging) and high-scoring (conceptual questions only, code + explanation, generate-then-comprehend). High scorers stayed cognitively engaged. ([Shen & Tamkin (arXiv)](https://arxiv.org/abs/2601.20245))

   5. **Productivity can be an illusion that hides cost.** Only ~20% of AI users (full delegators) were actually faster. AI users found the task easier but reported feeling "lazy" with "gaps in understanding" — AI-enhanced productivity is "not a shortcut to competence." ([Shen & Tamkin (arXiv)](https://arxiv.org/abs/2601.20245))

4. Skill atrophy

   1. **Higher trust in AI → less critical thinking.** In a survey of 319 knowledge workers (936 real GenAI examples), higher confidence in the AI predicted *less* critical thinking, while higher self-confidence predicted more. Routine offloading erodes the very judgment needed to catch AI errors. ([Lee et al., "The Impact of Generative AI on Critical Thinking," CHI 2025 (Microsoft Research)](https://www.microsoft.com/en-us/research/publication/the-impact-of-generative-ai-on-critical-thinking-self-reported-reductions-in-cognitive-effort-and-confidence-effects-from-a-survey-of-knowledge-workers/))

   2. **"Ironies of automation": the more you automate, the more the human skill that's still needed decays.** Bainbridge's classic result — automating a task leaves the operator out of practice, yet expected to take over precisely in the hard cases the automation can't handle. ([Bainbridge, "Ironies of Automation," 1983](https://www.ise.ncsu.edu/wp-content/uploads/2017/02/Bainbridge_1983_Automatica.pdf))

   3. **Automation complacency = monitoring skill decays with reliable tools.** Defined as "poorer detection of system malfunctions under automation compared with under manual control." High reliability makes operators disengage; it is *not* reduced by experience and is hard to train away. ([Automation bias/complacency (Parasuraman, Endsley)](https://en.wikipedia.org/wiki/Automation_bias))

   4. **Skill gains from AI don't persist once it's removed.** AI acts like an "exoskeleton": performance boosts on writing and technical tasks vanished when workers later worked unaided — the underlying skill was never built or retained. (Wu et al.; Wiles et al., cited in [Shen & Tamkin (arXiv)](https://arxiv.org/abs/2601.20245))

   5. **Novices are most exposed.** Less-experienced workers get the biggest productivity boost from AI — and are exactly the group still meant to be acquiring skills, so they have the most to lose to atrophy. ([Shen & Tamkin (arXiv)](https://arxiv.org/abs/2601.20245), [Lee et al., CHI 2025](https://www.microsoft.com/en-us/research/publication/the-impact-of-generative-ai-on-critical-thinking-self-reported-reductions-in-cognitive-effort-and-confidence-effects-from-a-survey-of-knowledge-workers/))

5. Brain fry

   1. **"AI brain fry" is a real, distinct phenomenon.** Defined as mental fatigue from excessive use or oversight of AI tools beyond one's cognitive capacity — a "fog" or "buzzing," trouble focusing, slower decisions, headaches. 14% of AI-using workers reported it (study of 1,488 U.S. workers). ([Bedard et al., "When Using AI Leads to 'Brain Fry'," HBR/BCG](https://hbr.org/2026/03/when-using-ai-leads-to-brain-fry))

   2. **Overseeing AI is the most taxing part.** Workers with high (vs low) AI oversight expended 14% more mental effort, 12% more mental fatigue, and 19% more information overload. Watching and double-checking agents is harder on the brain than doing the work. ([Bedard et al. (HBR)](https://hbr.org/2026/03/when-using-ai-leads-to-brain-fry))

   3. **More tools is not better past a point.** Productivity rose from one to two tools, less with a third, then dipped after three simultaneous tools — classic multitasking costs. ([Bedard et al. (HBR)](https://hbr.org/2026/03/when-using-ai-leads-to-brain-fry))

   4. **It carries real business costs.** Among those experiencing it: +33% decision fatigue, +11% minor errors, +39% major errors, and intent to quit jumped from 25% to 34% — often the heaviest users are top talent. ([Bedard et al. (HBR)](https://hbr.org/2026/03/when-using-ai-leads-to-brain-fry))

   5. **Brain fry ≠ burnout; management shapes it.** Burnout is emotional/physical exhaustion; brain fry is acute cognitive strain. Using AI to replace "toil" *lowered* burnout (~15%). Managers who answer AI questions → 15% lower fatigue; "figure it out yourself" → 5% higher. Rewarding token/line-count metrics makes it worse. ([Bedard et al. (HBR)](https://hbr.org/2026/03/when-using-ai-leads-to-brain-fry))