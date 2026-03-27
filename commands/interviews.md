# Discovery Interviews

> **Slash command template.** Copy this file to `.claude/commands/interviews.md` in your project root to enable the `/interviews` command.

You are presenting the available discovery interviews for this project. These interviews capture context that helps agents work effectively.

## Instructions

1. **Check completion status** for each interview by looking for the output file:

| # | Interview | Time | Output File | Purpose |
|---|-----------|------|-------------|---------|
| 1 | Developer Onboarding | 20-30 min | `~/.claude/CLAUDE.md` | Personal preferences, communication style |
| 2 | Product Discovery | 45-60 min | `_docs/PRODUCT.md` | Vision, users, features, business model |
| 3 | Workflow | 30-40 min | `_docs/WORKFLOW.md` | How work gets planned, built, reviewed, shipped |
| 4 | Coding Mindset | 15-20 min | Coding Philosophy section in `_docs/WORKFLOW.md` | Decision-making principles, technical philosophy |
| 5 | Design Discovery | 15-20 min | `_docs/DESIGN.md` | Visual identity, UI principles, accessibility |

2. **Check each output file** - if it exists and has substantive content (not just a placeholder), mark as done.

3. **Present the menu** showing status, then let the developer choose which to run (or skip).

4. **If the developer picks one**, read the corresponding template from `_docs/interviews/` and run the interview.

## Notes

- Not all interviews are needed for every project. A CLI tool doesn't need Design Discovery. A personal project may skip Workflow.
- Developer Onboarding is the most important — it shapes how the agent communicates across all projects.
- If critical interviews are missing, agents should mention it at session start but not block on it.
- Interviews can be re-run at any time to update the output documents.
