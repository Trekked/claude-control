# Workflow Interview

> **Reference template.** Run this interview once during project setup. Paste the contents into a Claude Code session to begin. Not typically used as a recurring slash command.

You are establishing the development workflow for a new project. The goal is to understand how work gets planned, built, reviewed, and shipped so you can follow the process and help improve it.

## Instructions

1. Read any existing project documentation for context
2. Conduct a conversational interview covering the topics below
3. Ask one question at a time, follow up on specifics
4. Challenge anything that seems unclear or contradictory - better to nail it down now
5. Write the results to two places:
   - **Transcript**: A file with verbatim Q&A (ask where to save)
   - **Synthesised document**: A `_docs/WORKFLOW.md` reference document agents will follow

## Questions

### Work Management (Q1-2)
1. **Tools** - How do you manage work? (GitHub Issues, Linear, Notion, Jira, etc.) What does a well-written ticket look like? Who writes the tickets?
2. **Project tracking** - Do you use a kanban board, sprints, or something else? What columns/states does work move through?

### Branching & Version Control (Q3-4)
3. **Branching strategy** - Feature branches off main? Release branches? Naming conventions? Is main always deployable?
4. **Commits** - Message conventions? (conventional commits, free-form?) Ticket numbers in commits? Single or multiple commits per PR?

### Pull Requests (Q5-7)
5. **PR creation** - What goes in a PR description? Template or free-form? How do you link PRs to tickets?
6. **PR size** - How big is too big? Do you prefer stacked PRs, feature flags, or large PRs?
7. **Merging** - Who merges? Squash, rebase, or merge commits? Any branch protection rules?

### Code Review (Q8-10)
8. **Review process** - Who reviews? How thorough? Line-by-line or approach-level?
9. **Automated reviews** - Do you use Copilot, CodeRabbit, or other AI review tools? How do you handle their feedback?
10. **Review feedback loop** - How should feedback be addressed? One commit per comment? Push after each fix or batch them?

### Testing (Q11-12)
11. **Testing philosophy** - What's the testing bar? TDD? Coverage targets? What types of tests matter most?
12. **Testing in the workflow** - Do tickets include test requirements? Are tests in the same PR or separate?

### Deployment (Q13-14)
13. **Environments** - What environments exist? (local, staging, preview, production) How do they relate?
14. **Deployment process** - Automatic or manual? How do database migrations get deployed? Any zero-downtime requirements?

### Process (Q15-18)
15. **Daily rhythm** - What does a typical productive day look like? How does work get picked up?
16. **Scope changes** - How do you handle scope changes mid-ticket? Abandoned work? Hotfixes?
17. **Technical debt** - How do you track and manage it? When do you stop to address it?
18. **When things go wrong** - Incident response? Post-mortems? Blameless culture?

### Agent-Specific (Q19-20)
19. **Agent autonomy** - When should agents just build vs stop and ask? What decisions can agents make independently?
20. **Handoffs** - How do agents pick up context between sessions? What should they re-read? How do you do standups and retros?

## Interview Style Guide

- Be specific - "how do you handle X" is better than "tell me about your process"
- When they say "it depends", ask for the cases
- Look for implicit rules that haven't been written down
- Ask about what's gone wrong in the past - that reveals what matters
- Challenge anything that sounds aspirational but might not be practical
- Test for contradictions (e.g., "small PRs" vs "complete features")

## Post-Interview

- Write a synthesised `_docs/WORKFLOW.md` covering the full lifecycle
- Include sections for: planning, branching, commits, PRs, review, testing, deployment, daily rhythm
- Add a coding philosophy section if the conversation covered it
- Use generic terms (developer, agent) instead of specific names for process steps
- Update project memory with key workflow rules
- Ask the developer to review and refine

## Adapting for Your Project

Consider adding sections specific to your setup:
- **Monorepo**: Package boundaries, cross-package changes, build/test scoping
- **Mobile**: App store submissions, versioning, beta distribution
- **Infrastructure**: Terraform/IaC workflow, environment provisioning
- **Open source**: Contribution guidelines, issue triage, release process
