# Ashby Agentic Engineering Article Summary

Article: "AI, Ashby Engineering, and the Future" (Colin, Head of EMEA Engineering at Ashby). A practitioner's view from a company where >50% of new production code is AI-generated.

## Most Important Findings

1. The cost of writing code is heading to zero; the cost of meaningful software is not.
Since August 2025, over half of Ashby's new production code is AI-generated, with no spike in customer issues and no regressions in quality, velocity, or onboarding (codebase comprehension reportedly went up). AI takes the mechanical parts (syntax, glue code); judgment and taste matter more, not less.

2. Two non-negotiable ground rules.
- Empathy cannot be replaced by AI. Products are a human endeavor; LLMs have no taste and don't know your customers. Write docs/specs for the humans who read them, don't let LLMs produce convincing-but-useless prose.
- You are responsible for what you ship. Whether hand-written or fully AI-generated, you must understand what the code does, why, and what happens when it breaks. The biggest risk isn't that AI is wrong, it's that it sounds right.

3. Think more, not less; skepticism must increase.
LLMs make it easy to "no-brain" through work. Ask for alternatives, edge cases, and self-critique. Running many agents in parallel is "multitasking on steroids", it feels productive but degrades the quality of your decisions and your understanding of what's being built.

4. Specs are still for humans.
What a human needs from a spec (focus on expensive-to-change decisions, the "why Redis not Postgres") differs from what an LLM needs. Keep writing specs for humans; LLMs can consume them as useful extra context.

5. Mental model: LLM as dice, not superintelligence.
Some tasks need no high roll (summarizing, pattern-finding). Some they'll never get right (precise counting/arithmetic). You can "load the dice" with good examples.

6. Two modes of working: sidekick vs delegate (the "blast radius" rule).
- Sidekick (you drive): high-risk work, migrations, PII, security, architecture. "Looks right" isn't good enough.
- Delegate (AI drives): low blast-radius work, prototypes, local/ops tools.
The real skill is knowing which mode you're in. Most engineers over-delegate first, then over-correct. The question isn't "should I use AI?" but "how much should I trust it here?"

7. Safety built into infrastructure, not imposed as discipline.
Ashby uses a "Swiss cheese" model: linters, Danger rules, tests, feature flags, observability, and AI-assisted review each catch what the others miss. They give generous token budgets but do NOT mandate AI use or measure token usage, because that "encourages slop."

8. Where the work is shifting.
- Code review: stop being "human linters"; focus on whether the change makes sense, risk areas, performance, and (critically) sensible abstractions. LLMs over-generate new code and avoid reuse, so pushing toward simplicity is now a top reviewer job.
- Verification is the new bottleneck: writing is cheap, so invest in tests and "AI reviewing AI" while keeping humans engaged on quality.
- Customer understanding is now a core engineering skill: engineers spend more time on session replays, interviews, and support conversations.

9. The codebase has a new audience.
LLMs read every name, pattern, and module boundary literally. A messy codebase now degrades every piece of AI code that touches it, so code quality compounds.

## 3 Questions for an Interactive Session (Software Teams)

1. For our recent AI-assisted work, were we in "sidekick" or "delegate" mode, and was that the right call?
Where did we delegate something high-blast-radius (migrations, security, architecture) that deserved us in the driver's seat?

2. What does "you are responsible for what you ship" actually require from us?
Can each of us explain what our AI-generated code does, why, and what happens when it breaks, or are we shipping things that merely "sound right"?

3. If writing code is now cheap, where should our effort go instead?
Are we still acting as "human linters" in review, or are we shifting toward abstractions, verification, and genuine customer understanding?