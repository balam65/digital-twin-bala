# AGENTS.md — Agent Injection & Skill Activation Guide

> Read `CONTEXT.md` first, then use this file to select the right skill and prompt for your task.

---

## Skill Selection Flow

```
What do I need to do?
        │
        ├── Evaluating or choosing between options?     → solution-strategy-formulation
        │
        ├── Creating something that doesn't exist yet?  → innovation-cross-domain-design
        │
        ├── Assessing a person's capability/potential?  → talent-discovery
        │
        ├── Helping someone who is stuck or blocked?    → mentorship-and-unblocking
        │
        └── Driving AI adoption or managing resistance? → agentic-workflow-advocacy
```

---

## Activation Guide

When approaching any task in this kernel, execute this decision chain first:

```
1. Problem Clarity   → Is the problem statement precise and validated? If not, stop and clarify.
2. Constraint Map    → What are the technical, business, and timeline constraints?
3. Skill Routing     → Which of the 5 skills applies? (see table below)
4. Depth Calibration → Is the audience technical or non-technical? Adjust output depth accordingly.
5. Trade-Off Check   → Does the output explicitly surface trade-offs, not just a recommendation?
6. Value Stream Tag  → Revenue / Risk / Cost — which does this output serve?
```

---

## Skill Reference Table

| Task | Skill File | Prompt File |
|---|---|---|
| Define the problem and map solution pathways | `skills/solution-strategy-formulation.md` | `prompts/solution-strategy.md` |
| Generate a novel solution from first principles | `skills/innovation-cross-domain-design.md` | `prompts/innovation-design.md` |
| Assess someone's talent and potential | `skills/talent-discovery.md` | `prompts/talent-discovery.md` |
| Unblock or mentor a stuck team member | `skills/mentorship-and-unblocking.md` | `prompts/mentorship-unblocking.md` |
| Guide a team toward AI/agentic adoption | `skills/agentic-workflow-advocacy.md` | `prompts/agentic-advocacy.md` |

---

## Consistency Rules for Agents

When generating or extending content in this kernel:

1. **Skill frontmatter is mandatory** — every `SKILL.md` must have `name`, `description`, `when-to-use` fields.
2. **Prompts must declare variables** — use `{{variable_name}}` format for all input placeholders.
3. **Problem-first sequencing** — every output must demonstrate that the problem was understood before solutions were generated.
4. **Trade-off transparency** — recommendations must include explicit trade-offs, not just conclusions.
5. **Audience calibration** — depth and vocabulary must match the stated audience (technical vs. business).
6. **Value stream tagging** — every significant output should be traceable to Revenue, Risk, or Cost value streams.

---

## Cross-Reference to Principles

All skills and prompts in this kernel are grounded in principles documented in [PHILOSOPHY.md](PHILOSOPHY.md).

Key principle-to-skill mappings:

| Principle | Primary Skill |
|---|---|
| First Principles Before Patterns | `innovation-cross-domain-design` |
| Symptoms vs. Root Problems | `solution-strategy-formulation` |
| Potential Over Pedigree | `talent-discovery` |
| Guided Discovery Over Direct Transfer | `mentorship-and-unblocking` |
| Inevitability & Early Leverage | `agentic-workflow-advocacy` |
