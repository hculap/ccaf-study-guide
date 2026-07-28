# CCAF Study Guide (910/1000): Your Last Cheat Sheet

Unofficial prep for **Claude Certified Architect - Foundations (CCAF)**. I scored **910/1000** on the exam and open-sourced the notes I used as my last cheat sheet.

The CCAF exam is scenario-heavy: you pick the right architecture when an agent forgets context, a generic tool keeps misfiring, or a customer escalation lands mid-process. The official guide covers all of it, but it's dense. This repo distills **30 exam tasks** across 5 domains into two complementary views: **what to do** (patterns and traps) and **what not to do** ([anti-patterns catalog](study/03-anti-patterns-catalog.md)).

**What's inside:** a one-page concept map, a trap taxonomy (why wrong answers sound right), and an **[anti-patterns catalog](study/03-anti-patterns-catalog.md)** that maps every "avoid / do not / instead of" warning from the official guide. If a distractor sounds plausible, check the traps first; if it sounds like a shortcut the guide rejects, check the anti-patterns.

Use this as your **last cheat sheet**, not your textbook. Take a mock first to see where you stand, then study the official guide and use this repo to close the gaps.

## Start here

1. Get access via [Anthropic Academy / Skilljar](https://anthropic.skilljar.com/claude-certified-architect-foundations-access-request)
2. Take a free mock ([CyberSkill](https://ccaf.cyberskill.world/) or [Certification Guide](https://claudecertificationguide.com/)) to baseline where you stand
3. Read the **official exam guide** at least **3 times** (I printed mine to cut digital distractions)
4. **Practice on a real project** alongside study: build an agent loop, wire up MCP tools, or configure Claude Code. Scenarios stick better when you've lived them.
5. Retake mocks until you hit **900+**, then book the real exam

Full workflow: [study/README.md](study/README.md)

## Study path


| Step | Doc                                                        | What you get                  |
| ---- | ---------------------------------------------------------- | ----------------------------- |
| 1    | [Concept map](study/00-concept-map.md)                     | All 30 tasks on one page      |
| 2    | [Mock exam trap guide](study/02-mock-exam-trap-guide.md)   | Why wrong answers sound right |
| 3    | [Anti-patterns catalog](study/03-anti-patterns-catalog.md) | What the guide says not to do |
| 4    | [API & product FAQ](study/04-api-and-product-faq.md)       | Exam vs production gotchas    |


**Domain weights:** Agentic Architecture (27%) · Tool Design & MCP (18%) · Claude Code Config (20%) · Prompt & Structured Output (20%) · Context & Reliability (15%). See the [concept map](study/00-concept-map.md) for task breakdown.

**Recommended Academy path:** Building with the Claude API → Claude Code in Action → Introduction to Agent Skills → Introduction to MCP.

## Trap cheat sheet

High-yield patterns from mock exams. Full taxonomy: [02-mock-exam-trap-guide.md](study/02-mock-exam-trap-guide.md).

```
Context filling up (multi-issue)     → 5.1 Summarize resolved; active thread full
Generic tool, inconsistent output    → 2.1 Split typed tools
Messy source formats                 → 4.3 Schema + normalization in prompt
Function behind wrappers             → 2.5 List aliases → grep each
Agent forgets mid-conversation       → 5.1 Pass full messages array
Unknown bug path                     → 1.6 Adaptive investigation
Long code exploration (30+ min)      → 5.4 Scratchpad file
Mid-process escalation               → 1.4 Structured handoff brief
Angry + no context                   → 5.2 Acknowledge + one question
Identity multi-match                 → 5.2 Ask identifiers, never guess
```

## More

- Community links and extra mocks: [resources/links.md](resources/links.md)
- Disclaimer: [DISCLAIMER.md](DISCLAIMER.md)
- License: MIT ([LICENSE](LICENSE))

