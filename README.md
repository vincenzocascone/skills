# Skills

## Installation

```sh
npx skills add vincenzocascone/skills
```

Or install manually — copy a skill's folder into your agent's skills directory (for Claude
Code: `~/.claude/skills/`), or zip it, rename to `<name>.skill`, and add it on claude.ai
under Settings → Capabilities → Skills.

## Skills

### navigator

Author-first learning mode. You write and debug the code yourself; the agent acts as
navigator — fundamentals-first primers, Socratic debugging, code review, explain-back
checkpoints — and does **not** write solutions in the territory you're learning. Agents
optimize for handing you working code, which is exactly wrong when the goal is learning:
reading generated code produces *recognition*, which feels like understanding but doesn't
survive contact with a real bug. Built for working far outside your home stack.

The protocol:

- **Blind vs. home territory** with per-concept depth tiers, and an explicit promotion
  mechanism — a concept stays "blind" until you pass its explain-back gate.
- **The authorship rule** — in blind territory you produce the first implementation *and its
  design* (schemas, decomposition, tests included); the agent drafts only home-territory
  code, tool glue, and instrumental code like debug visualizers.
- **Socratic-only debugging** — the agent helps you form hypotheses and gather evidence,
  never hands over the diagnosis; the evidence-gathering is yours too.
- **An escape hatch** — ask explicitly and the agent writes the piece after naming the
  trade-off in one sentence, no lecturing. Scoped per-piece; never standing permission.
- **Spaced review** — the skill creates and maintains a plain-markdown `LEARNING.md` ledger
  in your project (concept, tier, review log, next-due dates at expanding intervals) and opens
  sessions with retrieval questions from due concepts. The file is yours to read and hand-edit;
  agents only append to it.

To make the mode standing for a whole project rather than per-session, put its rules in the
project's agent-instructions file (`CLAUDE.md`, `AGENTS.md`, or your agent's equivalent —
loaded every session).
