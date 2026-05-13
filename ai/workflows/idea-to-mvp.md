# Workflow: Idea to MVP

## What this file is

This workflow describes how to move from a raw idea to a scoped MVP.

## Why this file exists

Projects often fail because they jump from idea directly to code.

This workflow forces the project to pass through discovery, product definition, architecture, and implementation planning.

## How to use

Ask your AI tool:

```txt
Use ai/workflows/idea-to-mvp.md.
Read ai/project/current-stage.md.
Activate only agents allowed for the current stage.
```

---

## Stage 0 — Intake

### Active agents
- orchestrator

### Goal
Clarify the project idea, business goal, audience, constraints, and desired outcome.

### Outputs
- project.md
- context.md
- current-stage.md

---

## Stage 1 — Market Discovery

### Active agents
- marketer
- ux-researcher
- product-manager

### Goal
Understand audience, market, pains, alternatives, and positioning.

### Outputs
- audience definition
- positioning
- assumptions
- validation experiments

---

## Stage 2 — Product Discovery

### Active agents
- product-manager
- ux-researcher
- marketer

### Goal
Turn market and user findings into product direction.

### Outputs
- product hypothesis
- user stories
- success metrics
- product boundaries

---

## Stage 3 — MVP Definition

### Active agents
- product-manager
- tech-architect

### Goal
Define the first implementation scope.

### Outputs
- PRD
- MVP scope
- backlog
- architecture draft

---

## Stage 4 — Technical Planning

### Active agents
- tech-architect
- developer

### Goal
Prepare implementation.

### Outputs
- architecture
- data model
- integrations
- implementation plan

---

## Stage 5 — Development

### Active agents
- developer
- qa

### Goal
Build and validate features.

### Outputs
- working implementation
- test plan
- release notes
