# Prompt: Solution Strategy Formulation

## Purpose
Guide a structured problem-solving session from pain-point identification through to a formulated, feasibility-assessed recommendation.

## When to Use
- A new feature, project, or business requirement needs a clear solution strategy.
- Multiple stakeholders have conflicting ideas about what to build.
- A problem exists but the root cause hasn't been clearly identified.

## Variables

| Variable | Description | Example |
|---|---|---|
| `{{problem_description}}` | The raw problem or request as stated by the stakeholder | "Our onboarding takes too long" |
| `{{requestor}}` | Who initiated this — end user, business, internal team | "Product Manager, on behalf of enterprise customers" |
| `{{current_state}}` | How the system or process works today | "Manual 5-step onboarding with email verification" |
| `{{constraints}}` | Known technical, business, or timeline limitations | "No new integrations; must ship in 6 weeks" |

## Prompt

```
You are applying the Solution Strategy Formulation framework.

Problem Description: {{problem_description}}
Requestor: {{requestor}}
Current State: {{current_state}}
Constraints: {{constraints}}

Execute the following phases:

## Phase 1: Context Gathering & Problem Definition
1. Identify the trigger: Who initiated this and what motivated it (pain point, inefficiency, feature gap, or incident)?
2. Capture the primary pain points: What are the exact issues? What is the impact (operational, user friction, cost)?
3. Distinguish symptoms from root problems: What is being reported vs. what is actually broken?
4. Map the current state: Where do breakdowns, bottlenecks, or workarounds occur?
5. List all constraints: Technical architecture, business rules, compliance, timeline, budget.
6. Validate understanding: State your refined problem definition and flag any assumptions that need stakeholder confirmation.

## Phase 2: Pathway Generation
Generate a minimum of 2 distinct solution pathways. Each pathway must:
- Represent a meaningfully different trade-off (e.g., speed vs. scalability, build vs. buy).
- Draw on known patterns, external benchmarks, or first principles as appropriate.
- Be described in 2–4 sentences.

## Phase 3: Feasibility Assessment
Evaluate each pathway against these criteria:

| Criterion | Pathway A | Pathway B |
|---|---|---|
| Feasibility (can it be built within constraints?) | | |
| Cost (effort + infrastructure + operations) | | |
| Time to Deliver | | |
| Scalability | | |
| Maintainability | | |
| Risk (technical uncertainty, dependencies) | | |

## Phase 4: Recommendation
- Select the most balanced option.
- State explicitly: Why this option? What trade-offs are accepted? Under what conditions would another option be better?

## Phase 5: Stakeholder Communication Summary
Produce a brief summary structured as:
- Problem
- Options evaluated
- Decision criteria
- Recommended option and rationale
```

## Expected Output
- Refined problem statement
- A minimum of 2 distinct solution pathways
- Comparative feasibility table
- A clear recommendation with stated trade-offs
- A stakeholder-ready summary
