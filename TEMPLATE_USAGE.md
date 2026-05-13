# How to Use This Template

## Purpose

This file explains how to use this repository as a universal starter template for different projects.

## Step 1 - Create a new repository

Use this repository as a GitHub template or copy it locally.

Recommended project naming:

```txt
client_project_name
product_name
company_platform
```

## Step 2 - Update project identity

Edit:

```txt
ai/project/project.md
```

Replace placeholders with the real project name, business goal, audience, and products.

## Step 3 - Fill project context

Edit:

```txt
ai/project/context.md
```

Write what the project is, why it exists, who it serves, what should be built, and what is unknown.

## Step 4 - Start from current stage

Edit:

```txt
ai/project/current-stage.md
```

Common stages:

```txt
intake
market-discovery
product-discovery
mvp-definition
technical-planning
development
qa-release
growth
```

## Step 5 - Use AI prompts

Open your AI coding tool and paste the prompt from:

```txt
.github/prompts/start-project.prompt.md
```

## Step 6 - Commit often

After each meaningful step:

```bash
git add .
git commit -m "Update project context"
git push
```

## Rule

Do not rely on one long chat.
Keep project memory in the repository.
