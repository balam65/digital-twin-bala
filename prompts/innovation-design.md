# Prompt: Innovation & Cross-Domain Solution Design

## Purpose
Synthesize a genuinely novel solution for a problem where no adequate established option exists, using first-principles decomposition and deliberate cross-domain exploration.

## When to Use
- Existing solutions are inadequate, too costly, or structurally misaligned with the problem.
- The problem is novel, ambiguous, or highly constrained.
- Standard pathway evaluation (Skill 1) has been attempted and found insufficient.

## Variables

| Variable | Description | Example |
|---|---|---|
| `{{problem_statement}}` | The core problem in its most precise form | "We need real-time inference under 100ms on edge devices with no connectivity" |
| `{{failed_approaches}}` | What has already been tried and why it failed | "Cloud inference failed due to latency; local models too large for device RAM" |
| `{{fundamental_domain}}` | The core domain or discipline governing the problem at its most fundamental level | "Human behaviour, incentive design, information asymmetry" |
| `{{constraints}}` | Hard limits that cannot be negotiated | "No new headcount, must work within existing regulatory framework, 90-day delivery window" |

## Prompt

```
You are applying the Innovation & Cross-Domain Solution Design framework.
This skill is used when existing solutions are inadequate. Do NOT repackage known solutions.

Problem Statement: {{problem_statement}}
Failed Approaches: {{failed_approaches}}
Fundamental Domain: {{fundamental_domain}}
Hard Constraints: {{constraints}}

Execute the following phases:

## Phase 1: First-Principles Decomposition
1. Strip away all assumptions tied to current implementations.
2. Identify the core scientific, mathematical, or system principles that govern this problem.
3. State the problem at its most fundamental level (not as a software problem — as a physics, information, or systems problem).

## Phase 2: Cross-Domain Exploration
Identify at least 3 unrelated domains or fields that solve an analogous fundamental problem.
For each domain:
- Describe the analogous problem.
- Describe how that domain solves it.
- Identify the transferable principle.

| Domain | Analogous Problem | Their Solution | Transferable Principle |
|---|---|---|---|
| | | | |
| | | | |
| | | | |

## Phase 3: Novel Solution Synthesis
Combine insights from Phase 1 and Phase 2.
Generate 1–3 novel solution concepts that:
- Did not exist in the original solution space.
- Emerge directly from the cross-domain synthesis.
- Have no direct benchmark (that is expected and acceptable).

For each concept: describe the mechanism, the core transferable insight it uses, and what remains uncertain.

## Phase 4: Risk & Iteration Plan
For each novel concept:
- What is the highest-uncertainty assumption that must be validated first?
- What is the simplest POC or experiment that would either confirm or eliminate this concept?
- What is the expected iteration cycle?
```

## Expected Output
- A first-principles restatement of the problem
- A cross-domain exploration table (min 3 domains)
- 1–3 novel solution concepts with mechanisms described
- POC / validation plan for each concept
