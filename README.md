# Claude Control

A set of templates, docs, and prompt interviews to help Claude work better with you and your project.

Developed during the [Trekked](https://trekked.com) project and documented on [trekked.dev](https://trekked.dev). These templates are project-agnostic — drop them into any repo and start building shared context with your AI agents.

## What's in the box

### Commands

Slash commands for Claude Code. Copy to `.claude/commands/` in your project.

| File | Command | Purpose |
|------|---------|---------|
| `commands/onboard.md` | `/onboard` | Developer preferences, communication style (20-30 min) |
| `commands/interviews.md` | `/interviews` | Menu of all interviews with completion tracking |

### Interviews

Discovery interviews run during project setup. The `/interviews` command reads these from `_docs/interviews/`.

| File | Time | Purpose | Output |
|------|------|---------|--------|
| `interviews/product-discovery.md` | 45-60 min | Vision, users, features, business model | `_docs/PRODUCT.md` |
| `interviews/workflow.md` | 30-40 min | Development process, PRs, deployment | `_docs/WORKFLOW.md` |
| `interviews/mindset.md` | 15-20 min | Coding philosophy, decision-making | Section in `_docs/WORKFLOW.md` |
| `interviews/design-discovery.md` | 15-20 min | Visual identity, UI principles | `_docs/DESIGN.md` |

## How to Use

### Quick start

Clone this repo as your project's `_docs` directory, then copy the commands:

```bash
git clone https://github.com/Trekked/claude-control.git _docs
mkdir -p .claude/commands
cp _docs/commands/*.md .claude/commands/
```

The `/interviews` command already looks for templates in `_docs/interviews/` — no path changes needed.

### Project structure

```
your-project/
  .claude/
    commands/
      interviews.md     # /interviews (menu)
      onboard.md        # /onboard (direct)
  _docs/                # This repo, cloned
    interviews/
      product-discovery.md
      workflow.md
      mindset.md
      design-discovery.md
```

### Getting started

1. **Run `/onboard`** first — it shapes how the agent communicates across all projects
2. **Run `/interviews`** to see what else is available and work through what matters
3. **Not all interviews are needed** — a CLI tool doesn't need Design Discovery, a personal project may skip Workflow

### Onboarding a new team member

1. Have them run `/onboard` to establish their personal preferences
2. Point them at existing project docs — no need to re-interview

## Tips

- **Take it slow** — these interviews are about building deep context, not checking boxes
- **Write incrementally** — save to files as you go in case of context loss
- **Review the output** — always have the human review synthesised documents before they become canonical
- **Update over time** — re-run interviews or update docs as the project evolves
- **Keep personal and project separate** — developer preferences go in `~/.claude/CLAUDE.md` (global), project docs go in the repo
- **No secrets** — never store credentials, API keys, or sensitive personal information in context files
