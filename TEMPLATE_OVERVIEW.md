# Multiagent Project Template

Universal AI-native project template for working with multiagent systems, AI coding tools, product discovery, architecture, and implementation.

This repository is designed to be used as a reusable template for new projects.

## What this template gives you

- A structured AI context layer.
- Reusable agent definitions.
- Reusable workflows.
- Project memory files.
- Product definition files.
- Prompt files for Codex / Cursor / Claude Code / other AI coding tools.
- Safe `.env` and `.gitignore` defaults.

## Recommended usage

For every new project:

1. Create a new repository from this template.
2. Rename the project in `ai/project/project.md`.
3. Fill in `ai/project/context.md`.
4. Start from `ai/project/current-stage.md`.
5. Ask your AI coding tool to read `.github/prompts/start-project.prompt.md`.

## Core idea

The chat is temporary memory.
The repository is long-term memory.

Use markdown files in `ai/project/` to store project decisions, assumptions, architecture, backlog, and product context.

## Recommended workflow

```txt
Work in AI session
-> update project files
-> commit
-> push
-> open new session when context gets large
-> AI rereads repository context
-> continue
```

## Main folders

```txt
ai/
  agents/       Reusable AI roles
  workflows/    Reusable project workflows
  project/      Project-specific memory and context

apps/           Product applications
packages/       Shared packages/modules
docs/           Business, product, and technical documentation
.github/prompts AI tool prompt templates
```
