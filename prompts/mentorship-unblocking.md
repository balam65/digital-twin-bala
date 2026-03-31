# Prompt: Mentorship & Unblocking

## Purpose
Guide a structured mentorship or unblocking session using the Socratic discovery model. Maximize the individual's learning while resolving their blocker.

## When to Use
- A team member is stuck on a problem and doesn't know where to start ("blank page").
- A team member has been stuck on the same issue for too long ("rabbit hole").
- Providing structural and design feedback during a peer review session.
- Deciding whether to guide someone vs. give them the direct answer.

## Variables

| Variable | Description | Example |
|---|---|---|
| `{{scenario}}` | The type of blocker: "blank-page", "rabbit-hole", "peer-review", or "general-mentorship" | "rabbit-hole" |
| `{{individual_level}}` | Their seniority or experience level | "Mid-level, 3 years experience" |
| `{{problem_context}}` | What they are working on and what is blocking them | "Implementing a real-time notification system; has spent 2 days trying to fix a race condition" |
| `{{deadline_pressure}}` | Is there a deadline or team dependency risk? | "Blocking another engineer; must resolve by end of day" |

## Prompt

```
You are applying the Mentorship & Unblocking framework.
Your default mode is guided discovery (Socratic). Override to direct answer ONLY if deadline_pressure is critical.

Scenario: {{scenario}}
Individual Level: {{individual_level}}
Problem Context: {{problem_context}}
Deadline Pressure: {{deadline_pressure}}

## Step 1: Apply the Tell vs. Guide Decision
Given the deadline pressure, is this a "Guide" or "Tell" session?
- If "Guide" → proceed with Socratic questioning throughout.
- If "Tell" → be explicit that you are giving the answer due to constraints, and offer to revisit the methodology afterward.

## Step 2: Scenario-Specific Unblocking

### If scenario = "blank-page":
1. Ask them to explain the goal in their own words.
2. Ask them to state what they already know vs. what they don't know.
3. Help them break the problem into components.
4. Provide a *starting direction*, not a full solution.

### If scenario = "rabbit-hole":
1. Ask them to step away from the current approach entirely.
2. Ask: "What exactly are you trying to achieve?" / "What assumptions are you making?" / "What have you tried and why did it fail?"
3. Zoom out to the system level — is the issue in the implementation, or in the understanding of the problem?
4. Propose a different angle or suggest a reset.

### If scenario = "peer-review":
Review the work with this priority order:
1. Design and structural logic (highest priority).
2. Performance and maintainability implications.
3. Clarity and readability.
4. Skip minor stylistic issues unless they materially impact the above.
For each concern: explain *why* it is a problem, not just *that* it is a problem. Offer an alternative with trade-offs explained.
Calibrate challenge level: junior = build the mental model; senior = challenge the foundational decisions.

### If scenario = "general-mentorship":
Use Socratic questioning to uncover their blind spot. Ask: "What would you do if X assumption were wrong?" or "What outcome are you optimizing for?"

## Step 3: Output
Produce:
- The 3 most important questions to ask this person right now.
- A suggested re-framing of their problem (if applicable).
- Your recommendation on their next concrete step.
- Flag whether this requires a follow-up session.
```

## Expected Output
- Tell vs. Guide decision with rationale
- 3 targeted Socratic questions
- Problem reframe (if needed)
- Concrete next step recommendation
