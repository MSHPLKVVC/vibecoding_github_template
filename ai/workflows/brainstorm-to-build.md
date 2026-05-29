# Workflow: Brainstorm to Build

## What this file is

This workflow keeps product thinking, concept decisions, implementation tasks, and commits in one loop inside this repository.

It is inspired by the useful parts of agentic skill systems such as Superpowers: brainstorm before building, write down the concept, make a clear plan, implement in small slices, verify before calling work done.

## Why this file exists

The product should not be shaped in a separate ChatGPT thread and then handed to the coding agent as disconnected tasks.

The better loop is:

```text
Brainstorm here
-> fix the concept here
-> turn it into tasks here
-> implement here
-> verify here
-> commit here
```

## Operating Principles

- Do not jump straight to code when the user is still exploring the product idea.
- Keep the conversation casual, but make decisions concrete before implementation.
- Capture durable decisions in `ai/project/decisions.md`, `ai/project/backlog.md`, or product docs when they change future work.
- Prefer small vertical slices that can be opened in the browser and reacted to.
- Verify with `npm.cmd run build` and `npm.cmd run typecheck` for web changes.
- Commit completed slices with a clear message.

## Phase 1 - Brainstorm

Use when the user is reacting to screens, product logic, wording, UX flow, or strategy.

The assistant should:

1. Reflect the user's raw feedback in clearer product language.
2. Separate immediate fixes from backlog ideas.
3. Identify contradictions or missing decisions.
4. Ask only the questions that materially change the implementation.
5. Avoid turning every thought into code immediately.

Expected output:

- A short list of product decisions.
- A short list of concrete changes for the next slice.
- A parking-lot list for later ideas.

## Phase 2 - Concept Lock

Use when the direction is clear enough to build.

The assistant should state:

- What experience we are improving.
- What the screen or feature should help the user understand or do.
- What is intentionally out of scope.
- What will count as successful in the browser.

Keep this short enough that the user can correct it quickly.

## Phase 3 - Task Slice

Turn the concept into a buildable slice.

Each slice should include:

- UI changes.
- Data/model changes.
- Persistence behavior.
- Tests or verification.
- Commit boundary.

Avoid plans that require many unrelated decisions before the user can see progress.

## Phase 4 - Build

Implement the agreed slice.

The assistant should:

1. Read the relevant code first.
2. Make scoped edits.
3. Keep existing patterns unless there is a good reason to change them.
4. Run verification.
5. Restart the local dev server if needed.

## Phase 5 - Review and Commit

Before finishing:

1. Summarize what changed in product terms.
2. Mention verification results.
3. Commit the slice unless the user asked not to.
4. Leave the next obvious product question or next slice visible.

## Backlog Handling

When the user mentions useful but non-immediate ideas, add them to `ai/project/backlog.md`.

Examples:

- dashboard block customization;
- drag-and-drop layout;
- richer fund editing;
- backend persistence;
- Telegram bot flows.

## Current Product Fit

For Family Money Day System, this workflow is the default collaboration loop:

- brainstorm the family finance system directly in chat;
- lock the concept in project memory;
- build web slices quickly;
- later connect Telegram and durable storage.
