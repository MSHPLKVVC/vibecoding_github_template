# New Session Prompt

## What this file is

This prompt helps restart work after a previous AI session became too large.

## Why this file exists

AI chat context is temporary. Repository context is persistent.

Use this prompt when opening a new session.

---

Read the repository context and continue from the latest committed state.

Start with:
- README.md
- TEMPLATE_USAGE.md
- ai/project/project.md
- ai/project/context.md
- ai/project/current-stage.md
- ai/project/decisions.md
- ai/project/assumptions.md
- ai/project/backlog.md
- ai/project/architecture.md

Then:
1. Summarize what the project is.
2. Summarize the current stage.
3. Summarize the most important decisions.
4. Ask what task we should continue with, unless the task is already provided.
