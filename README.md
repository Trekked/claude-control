# Claude Control

A set of templates, docs, and prompt interviews to help Claude work better with you and your project.

Developed during the [Trekked](https://trekked.com) project and documented on [trekked.dev](https://trekked.dev). These templates are project-agnostic — drop them into any repo and start building shared context with your AI agents.

## Templates

### Discovery Interviews

| Template | Time | Purpose | Output | Blog Post |
|----------|------|---------|--------|-----------|
| `templates/onboard.md` | 20-30 min | Developer preferences, communication style | `~/.claude/CLAUDE.md` (global) | [The Travel Agents Part 2 — The Interview](https://trekked.dev/the-travel-agents-part-2) |

More templates coming soon — product discovery, workflow, design, and more. Follow along on [trekked.dev](https://trekked.dev).

## How to Use

### Quick start

Copy the templates you want into `.claude/commands/` in your project root to use them as slash commands:

```bash
# Copy a single template
cp templates/onboard.md your-project/.claude/commands/onboard.md

# Then in Claude Code
/onboard
```

### Project structure

```
your-project/
  .claude/
    commands/
      onboard.md       # /onboard
```

### For a new project

1. **Copy the templates** you need into `.claude/commands/`
2. **Developer Onboarding** is the most important — do it first
3. **Not all interviews are needed** — pick what matters for your project

### For onboarding a new team member

1. Have them run `/onboard` to establish their personal preferences
2. Point them at existing project docs — no need to re-interview

## Tips

- **Take it slow** — these interviews are about building deep context, not checking boxes
- **Write incrementally** — save to files as you go in case of context loss
- **Review the output** — always have the human review synthesised documents before they become canonical
- **Update over time** — re-run interviews or update docs as the project evolves
- **Keep personal and project separate** — developer preferences go in `~/.claude/CLAUDE.md` (global), project docs go in the repo
