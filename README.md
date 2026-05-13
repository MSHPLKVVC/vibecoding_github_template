# Multiagent Project Template

Universal AI-native repository template for building products with multiagent workflows, AI coding tools, and persistent project memory.

This template helps structure projects around:

* AI agents
* reusable workflows
* project memory
* architecture
* product discovery
* implementation planning
* long-term repository context

Instead of relying on one huge AI chat, the repository becomes the long-term memory system for the project.

---

# Why this exists

Most AI-assisted development becomes chaotic because:

* context windows overflow;
* chats become too large;
* decisions are forgotten;
* architecture drifts;
* requirements become inconsistent.

This template solves that by storing project context directly in the repository.

The repository becomes:

* persistent memory;
* workflow engine;
* project operating system;
* AI coordination layer.

---

# Core Idea

```txt id="t04oyh"
Chat/session = temporary memory
Repository = long-term memory
```

AI agents can restart, reread the repository, and continue working without relying on old chat history.

---

# What's Included

```txt id="m9h6oi"
ai/
  agents/        reusable AI roles
  workflows/     reusable project workflows
  project/       persistent project memory

apps/            product applications
packages/        shared modules
docs/            business/product/technical docs
.github/prompts reusable prompts for AI coding tools
```

---

# Included Agents

Examples:

* orchestrator
* marketer
* ux-researcher
* product-manager
* ui-designer
* tech-architect
* developer
* qa
* learning-experience-designer

---

# Included Workflows

Examples:

* idea-to-mvp
* feature-delivery
* landing-creation

---

# How to Use

## 1. Create a new repository from this template

Use GitHub template mode or clone/copy the repository.

---

## 2. Update project identity

Edit:

```txt id="69w0fx"
ai/project/project.md
```

Replace placeholders with your real project information.

---

## 3. Fill project context

Edit:

```txt id="wpr8p4"
ai/project/context.md
```

Describe:

* what the project is;
* who it serves;
* what should be built;
* constraints;
* known assumptions.

---

## 4. Set the current stage

Edit:

```txt id="6v53vg"
ai/project/current-stage.md
```

Examples:

```txt id="s5cxmb"
intake
market-discovery
product-discovery
mvp-definition
technical-planning
development
qa-release
growth
```

---

## 5. Open your AI coding tool

Examples:

* Cursor
* Codex
* Claude Code
* Copilot
* Windsurf

Paste the prompt from:

```txt id="e76i1q"
.github/prompts/start-project.prompt.md
```

The AI will:

* read repository context;
* detect current stage;
* activate relevant agents;
* continue project work.

---

# Recommended Workflow

```txt id="mlxb9m"
Work in AI session
-> update project files
-> commit
-> push
-> open new session when context gets large
-> AI rereads repository context
-> continue
```

---

# Recommended Repository Strategy

Use one monorepo per business/project.

Inside the monorepo:

* multiple apps/products;
* shared packages;
* shared AI context;
* shared workflows.

Example:

```txt id="kjlwmr"
apps/
  landing/
  crm/
  telegram-bot/

packages/
  shared/
  database/
  integrations/

ai/
  agents/
  workflows/
  project/
```

---

# Environment Variables & Security

This template includes:

* `.env.example`
* `.gitignore`

Never commit:

* `.env`
* secrets
* API keys
* production credentials

Only commit:

* `.env.example`

---

# Philosophy

This repository is not just code structure.

It is:

```txt id="9fjlwm"
AI-native project infrastructure
```

The goal is to make:

* AI collaboration scalable;
* project context persistent;
* workflows structured;
* implementation reproducible;
* long-term development manageable.

---

# Recommended Usage

Good for:

* startups
* SaaS
* internal tools
* AI products
* LMS platforms
* CRM systems
* bots
* marketplaces
* automation systems
* multi-product platforms

---

# License

MIT
