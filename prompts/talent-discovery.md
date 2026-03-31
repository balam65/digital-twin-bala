# Prompt: Talent Discovery

## Purpose
Evaluate a candidate's or team member's potential using a heuristic-based framework that prioritizes raw thinking ability and learning agility over credentials or specific experience.

## When to Use
- Evaluating candidates during an interview process.
- Assessing a team member's suitability for a more complex or ambiguous role.
- Building a hiring rubric or interview guide for a specific role.

## Variables

| Variable | Description | Example |
|---|---|---|
| `{{role}}` | The role or context being evaluated for | "Senior Product Designer, joining an AI-first team" |
| `{{candidate_background}}` | Brief description of their stated experience | "5 years at a fintech firm, led design for mobile apps" |
| `{{key_behaviors_observed}}` | What you have seen or heard during the interaction | "Answered questions quickly without clarifying scope. Strong visual portfolio." |
| `{{domain_context}}` | The type of problems they will face in the role | "Ambiguous, fast-moving, AI-augmented design decisions with no established playbook" |

## Prompt

```
You are applying the Talent Discovery framework to assess potential over pedigree.

Role: {{role}}
Candidate Background: {{candidate_background}}
Behaviors Observed: {{key_behaviors_observed}}
Domain Context: {{domain_context}}

Execute the following assessment:

## Phase 1: Green Flag Scan
Review the behaviors observed. For each green flag category, state whether there is positive, neutral, or absent evidence:

| Green Flag | Evidence | Signal Strength |
|---|---|---|
| Structured thinking — broke down problem before solving | | |
| Foundational understanding — reasoned from principles, not patterns | | |
| Learning agility — admitted gaps and proposed how to find answers | | |
| Ownership — took responsibility for past decisions including failures | | |
| Depth over surface — used real context, explained the "why" | | |

## Phase 2: Red Flag Scan
| Red Flag | Evidence | Risk Level |
|---|---|---|
| Buzzword usage without mechanical understanding | | |
| Jumped to solutions without clarifying the problem | | |
| Defensive when decisions were challenged | | |
| Blamed external factors without self-reflection | | |
| Rigidity — over-reliance on specific past tools or methods | | |

## Phase 3: Litmus Test Design (if interview not yet complete)
Propose one open-ended, slightly ambiguous scenario relevant to the role.
The scenario must:
- Have no obvious correct answer.
- Require the candidate to ask clarifying questions to proceed.
- Reveal how they decompose and handle uncertainty.

State what you are specifically watching for in their response.

## Phase 4: Potential vs. Pedigree Judgment
Based on the above:
1. How does their demonstrated thinking quality compare to the role's complexity demands?
2. Where are the genuine gaps — and are these gaps in knowledge (learnable) or mindset (structural)?
3. State your recommendation: Strong Yes / Yes with development plan / No — and your reasoning.
```

## Expected Output
- Green flag and red flag assessment tables
- Litmus test scenario (if applicable)
- Overall judgment with explicit reasoning on potential vs. pedigree trade-off
