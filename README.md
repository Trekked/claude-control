# Claude Control

A set of templates, docs, and prompt interviews to help Claude work better with you and your project.

Developed during the [Trekked](https://trekked.com) project and documented on [trekked.dev](https://trekked.dev). These templates are project-agnostic — drop them into any repo and start building shared context with your AI agents.

## Templates

### Discovery Interviews

Run these during project setup to build context. Use `/interviews` to see which are complete and pick one to run.

| Template | Time | Purpose | Output | Blog Post |
|----------|------|---------|--------|-----------|
| `templates/onboard.md` | 20-30 min | Developer preferences, communication style | `~/.claude/CLAUDE.md` (global) | [The Travel Agents Part 2 — The Interview](https://trekked.dev/the-travel-agents-part-2) |
| `templates/product-discovery.md` | 45-60 min | Product vision, users, features, business model | `_docs/PRODUCT.md` | |
| `templates/workflow.md` | 30-40 min | Development process, GitHub flow, deployment | `_docs/WORKFLOW.md` | |
| `templates/mindset.md` | 15-20 min | Coding philosophy, decision-making, trade-offs | Section in `_docs/WORKFLOW.md` | |
| `templates/design-discovery.md` | 15-20 min | Visual identity, UI principles, accessibility | `_docs/DESIGN.md` | |

### Menu Command

| Template | Purpose |
|----------|---------|
| `templates/interviews.md` | Menu of discovery interviews with completion status — run via `/interviews` |

## How to Use

### Quick start

Copy the templates you want into `.claude/commands/` in your project root to use them as slash commands:

```bash
# Copy all templates
cp templates/*.md your-project/.claude/commands/

# Or copy specific ones
cp templates/onboard.md your-project/.claude/commands/onboard.md

# Then in Claude Code
/interviews    # See the menu
/onboard       # Run directly
```

### Project structure

```
your-project/
  .claude/
    commands/
      interviews.md        # /interviews (menu)
      onboard.md           # /onboard
  _docs/
    templates/             # Interview templates (referenced by /interviews)
      product-discovery.md
      workflow.md
      mindset.md
      design-discovery.md
```

The `/interviews` command looks for templates in `_docs/templates/` by default. If you store them elsewhere, update the paths in `interviews.md`.

### For a new project

1. **Copy the templates** you need into `.claude/commands/` and `_docs/templates/`
2. **Run `/interviews`** to see what's available and start with what matters most
3. **Developer Onboarding** is the most important — do it first
4. **Not all interviews are needed** — a CLI tool doesn't need Design Discovery, a personal project may skip Workflow

### For onboarding a new team member

1. Have them run `/onboard` to establish their personal preferences
2. Point them at existing project docs — no need to re-interview
3. Run the mindset interview only if they have significantly different coding philosophies

## Tips

- **Take it slow** — these interviews are about building deep context, not checking boxes
- **Write incrementally** — save to files as you go in case of context loss
- **Review the output** — always have the human review synthesised documents before they become canonical
- **Update over time** — re-run interviews or update docs as the project evolves
- **Keep personal and project separate** — developer preferences go in `~/.claude/CLAUDE.md` (global), project docs go in the repo
- **No secrets** — never store credentials, API keys, or sensitive personal information in context files. Stick to work preferences and communication style
