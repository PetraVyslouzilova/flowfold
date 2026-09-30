# Flowfold

**Know when you can stop. Never lose the thread.**

Flowfold is a humane stopping skill for AI conversations. It notices natural places to pause, preserves open threads, reduces AI-generated “one more thing” momentum, and makes it easy to resume later.

> **Never tell people to stop. Make it safe to stop.**

## Why

AI conversations have no natural ending. One answer creates another question; one useful idea opens three more. Flowfold is designed for the moment when the work is valuable but the session does not need to continue forever.

It does **not** force breaks, diagnose hyperfocus, or tell people when to sleep. It creates an exit ramp without dropping the thread.

## What it does

- Detects natural stopping points instead of using a blunt timer.
- Notices when optional branches are multiplying.
- Watches for AI-generated momentum — when the assistant itself keeps creating new reasons to continue.
- Adds a gentle **Night Mode**: from 23:00 local time it looks for the next safe stopping point; around midnight it may offer one final time-based check.
- Switches to a low-FOMO mode late at night instead of constantly proposing new tangents.
- Produces a tiny checkpoint: **Done / Open / Next / Resume**.
- Respects “Keep going” without nagging.

## Example

> **Good place to fold.**  
> We’ve finished the main task and opened two new threads. I can save them here so you can resume without losing the thread.  
> **Fold here · Keep going**

If the user folds:

> ### Flowfold ✓
> **Done:** Chosen the project name and V1 behavior.  
> **Open:** README and launch post.  
> **Next:** Draft the final skill package.  
> **Resume:** `Continue from the Flowfold checkpoint and draft the release.`

## Install / use

Flowfold follows the open Agent Skills format: a skill is a folder anchored by `SKILL.md`.

Copy the `flowfold` folder into a skills/capabilities directory supported by your agent environment, or package the folder as a zip where the zip contains a single top-level `flowfold/` directory.

Then ask the agent to use the **flowfold** skill, or let the agent discover it from its name and description.

## Files

```text
flowfold/
├── SKILL.md
├── README.md
├── LICENSE
└── references/
    └── examples.md
```

## Design principles

1. **Agency over enforcement.**
2. **Natural boundaries over timers.**
3. **Time can increase sensitivity; it never forces a stop.**
4. **The assistant must stop manufacturing FOMO.**
5. **A fold must be shorter than the work it helps pause.**
6. **Never promise persistence the environment cannot guarantee.**

## Status

V1 — ready for public testing. Feedback and edge cases are welcome.

## License

MIT
