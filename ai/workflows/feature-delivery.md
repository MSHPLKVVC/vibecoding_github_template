# Workflow: Feature Delivery

## What this file is

This workflow describes how to deliver a single feature from request to implementation.

## Why this file exists

Feature work should not start with code. It should move through scope, impact analysis, implementation, and QA.

## Inputs

- Feature request.
- PRD.
- Architecture.
- Existing codebase.
- Backlog.

## Steps

1. If the request is still exploratory, use `ai/workflows/brainstorm-to-build.md` first.
2. Product Manager clarifies scope.
3. UX Researcher or UI Designer reviews user impact if needed.
4. Tech Architect reviews architecture impact.
5. Developer creates implementation plan.
6. Developer implements feature.
7. QA validates functionality.
8. Orchestrator updates backlog and decisions.
9. Commit the completed slice unless the user explicitly asks not to.

## Expected output

- Clear feature scope.
- Implementation plan.
- Code changes.
- Test plan.
- Updated documentation if necessary.
