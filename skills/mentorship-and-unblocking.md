---
name: Mentorship & Unblocking
description: Guides team members through technical blockers and ambiguity using a guided-discovery approach, maximizing learning and self-sufficiency.
when-to-use: Use this when a team member is stuck, tunnel-visioned, facing a 'blank page', or when conducting structural and architectural peer reviews.
---

# Mentorship & Unblocking

## Objective
To unblock team members while actively maximizing their learning and self-sufficiency, prioritizing structural understanding and problem decomposition over simply supplying the final answer.

## Core Philosophy: The Multiplier Effect
- **Guided Discovery:** Default to asking questions that lead the mentee to uncover the answer themselves (Socratic approach).
- **Learning > Speed:** Prioritize the building of robust mental models over fast resolution, unless external constraints require an immediate fix.
- **Structural Focus:** Emphasize design, structure, and underlying logic over minor stylistic details during reviews.

## 1. Resolving the "Blank Page" Scenario
When a team member does not know how or where to begin a problem:
1. **Verbalize the Problem:** Ask them to articulate the problem entirely in their own words.
2. **Boundary Identification:** Push them to explicitly list outline:
   - What they *do* know.
   - What they *do not* know.
   - What the successful end state looks like.
3. **Decomposition:** Help them break the monolithic problem down into smaller, achievable components.
4. **Direction, Not Solution:** Provide an initial starting vector (e.g., *"Start by figuring out X"*) rather than mapping out the full architecture or solution path.

## 2. Breaking the "Rabbit Hole" Fixation
When a team member has been stuck too long and is heavily tunnel-visioned on a single failing approach:
1. **Interrupt the Loop:** Ask them to step completely away from the current path and re-explain the core problem from scratch.
2. **Reframe via Questioning:**
   - *"What exactly are you trying to achieve at a high level?"*
   - *"What specific assumptions are baked into your current approach?"*
   - *"What approaches have you already tried, and why did they fail?"*
3. **System-Level Zoom Out:** Help them elevate their perspective back to the system level. (Often the issue is a fundamental misunderstanding of the problem itself, rather than a failure of execution).
4. **Pivot or Pause:** Suggest an entirely different angle of attack, or recommend a complete mental reset/break to shatter the fixation.

## 3. The "Tell vs. Guide" Decision Matrix
*Default Path:* Use Socratic questioning to uncover knowledge gaps and promote productive struggle.

*Intervention Path (Provide the Answer) Triggers:*
- The cost of delay is exceptionally high (e.g., critical deadline, blocking multiple other engineers).
- The person is completely hard-stuck with zero forward progress for an extended period.
- The intrinsic learning value of the struggle is incredibly low compared to the time being lost.

## 4. Architectural & Logic Review Mentorship
Treat peer reviews primarily as teaching opportunities rather than mere quality control gates. (Particularly since syntax and styling can be handled by AI tooling).
- **Explain the "Why":** Highlight exactly *why* a design choice is problematic, rather than just pointing out the error.
- **Provide Alternatives:** Suggest alternative patterns and explicitly explain the trade-offs of each option.
- **Ignore the Noise:** Let small stylistic issues slide as long as they do not materially impact maintainability, performance, or clarity.
- **Tailor the Challenge:**
  - *For Junior Candidates:* Prioritize the patient building and reinforcing of their core mental models.
  - *For Stronger Candidates:* Aggressively challenge their foundational decisions and push them to defend their trade-offs.
