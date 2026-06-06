# Cognitive Debt Paper Summary

## Most Important Findings

1. AI shifts the main software risk, not just speed.
The paper argues risk is moving from classic technical debt toward two less visible debts:
- Cognitive debt: team-level erosion of shared understanding.
- Intent debt: missing or stale goals, constraints, and decision rationale.

2. Triple debt model explains software health.
Software health depends on three layers staying aligned:
- Intent (what system is for)
- Code (how system is built)
- Shared understanding (how team reasons about change)
When one layer degrades, the others degrade too.

3. GenAI can reduce technical debt while increasing cognitive and intent debt.
AI can help with refactoring, tests, and code quality, but teams may accept generated code faster than they can understand it or capture why decisions were made.

4. Cognitive surrender is a key mechanism.
Teams may rely on plausible AI output with too little scrutiny, reducing deep reasoning and creating false confidence. This makes debt hard to see until changes start failing.

5. Cognitive debt signals in practice.
Common warning signs:
- Resistance to changing code
- Surprising side effects from "simple" changes
- Slow onboarding despite docs
- Loss of who-knows-what across team
- Low bus factor

6. Intent debt becomes critical with AI agents.
If goals, constraints, and rationale are not externalized, both people and agents optimize for the wrong thing. Systems drift from user needs even if tests pass.

7. Strong recommendation: treat understanding as a deliverable.
The paper recommends "intent-first" workflows and explicit team practices such as walkthroughs, ADRs, BDD/specs, retrospectives, and regular checks for drift between intended and actual behavior.

## 3 Questions for an Interactive Session (Software Teams)

1. Where are we currently trading understanding for speed?
Which recent AI-assisted changes shipped quickly, but left parts of the team unsure how or why they work?

2. If key people were unavailable next month, what would break first?
What does that reveal about our cognitive debt (shared understanding) and our bus factor?

3. Which critical product intents are not explicit today?
Where are goals, constraints (performance, security, accessibility, privacy), or decision rationales still "in people" instead of artifacts that both humans and AI can use?