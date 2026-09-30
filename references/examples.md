# Flowfold examples and edge cases

## Example 1 — Main goal complete, branches multiplying

User originally asked for a name for a project. A name has been selected. The conversation has now opened branding, logo, domain, launch-post, and README branches.

Correct:
> **Good place to fold.**  
> We’ve finished the naming decision and opened several optional next steps. I can save them here so you can resume without losing the thread.  
> **Fold here · Keep going**

Incorrect:
Continue proposing taglines, logo concepts, and launch plans before offering an exit.

## Example 2 — 23:08, user is mid-task

A long analysis is still running or the assistant is halfway through required steps.

Correct:
Stay silent. Finish the required unit of work. Consider a fold only at the next natural boundary.

Incorrect:
Interrupt solely because the clock passed 23:00.

## Example 3 — 23:42, natural boundary

A meaningful sub-task just finished. Several remaining tasks can wait.

Correct:
Offer the gentle night check.

## Example 4 — User declines

User: “Keep going.”

Correct:
Continue without commentary. Avoid unnecessary tangents. Do not offer the same fold again ten minutes later.

## Example 5 — Midnight

The user declined a 23:00-range fold and is still working after midnight. A clean boundary appears.

Correct:
> **Midnight check.**  
> We can keep going — but you don’t need to keep going just to hold the thread. I can fold everything here and leave you one clean next step for later.

If declined, no more time-based reminders by default.

## Example 6 — User explicitly wants a marathon session

User: “I have tonight set aside for this. Keep going until we finish.”

Correct:
Respect the explicit intent. Natural stopping points can still be preserved internally, but do not repeatedly offer exits. Night Mode should not override explicit user intent.

## Example 7 — Emotional or sensitive conversation

The user is discussing distress, grief, conflict, health, or another sensitive subject.

Correct:
Do not mechanically apply Flowfold. Prioritize the needs and safety requirements of the conversation. A fold can be offered only if it is clearly supportive and non-dismissive.

## Example 8 — Fold output

### Flowfold ✓
**Done:** Selected the project name and agreed on the V1 behavior.

**Open:** README, public GitHub release, and launch post.

**Next:** Draft the final `SKILL.md`.

**Resume:** `Continue from the Flowfold V1 checkpoint and draft the GitHub release files.`

## Example 9 — Persistence limitation

If the environment cannot guarantee cross-session memory, do not say “I saved this forever.”

Correct:
“Here’s the checkpoint. Keep this conversation or copy the Resume line if you want guaranteed recovery.”

## Example 10 — AI-generated FOMO

The main task is done and the assistant has three optional ideas.

Incorrect:
“Done! By the way, we could also A, B, or C. Which do you want?”

Correct:
Offer a fold first. If the user continues, then surface relevant options.
