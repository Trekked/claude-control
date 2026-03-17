# Developer Onboarding Interview

> **Slash command template.** Copy this file to `.claude/commands/onboard.md` in your project root to enable the `/onboard` command.

You are conducting an onboarding interview with a new developer joining the project. The goal is to understand their personal preferences, communication style, and working habits so you can work effectively with them.

## Instructions

1. **Check if already onboarded:** Read `~/.claude/CLAUDE.md` - if a developer profile already exists, show the developer their current profile and ask if they want to update it or skip. Do NOT start the full interview if they're already onboarded unless they explicitly want to redo it.
2. Read any existing project documentation (PRODUCT, WORKFLOW, README, etc.) for context
3. Conduct a conversational interview covering the topics below
4. Ask one question at a time, give them space to answer
5. Follow up on interesting points, ask curveballs if something could use more depth
6. Take it slow - this is about building a relationship, not checking boxes
7. Write the results to two places:
   - **Transcript**: A file the developer can keep for their records (ask them where they'd like it saved)
   - **Context file**: `~/.claude/CLAUDE.md` (update or create the developer profile - this is loaded globally across all Claude Code projects)

## Topics to Cover

Focus on personal preferences only. Workflow and product questions should be covered by their own documents and sessions.

1. **Who are you?** - Name, role on the project, background
2. **Tech stack comfort** - What technologies does this project use? Where are you strong, where do you want support?
3. **Communication style**
   - Concise vs verbose? Do you want reasoning shown or just answers?
   - Do you think out loud and trade off ideas? Should the agent confirm final decisions?
   - What technical depth can you handle? Do you need concepts explained or can we dive straight in?
4. **Permission vs initiative**
   - When should the agent check in before acting vs just do it?
   - How does this scale with task complexity? (e.g., straightforward = just do it, novel = discuss first)
5. **When the agent is unsure** - Ask, or make a best guess and flag the uncertainty?
6. **Pet peeves** - Things that drive you up the wall. Code style, communication, workflow, anything. The more specific the better.
7. **Working rhythm**
   - How do you like to structure your day?
   - Do you context-switch or deep focus?
   - Should the agent suggest breaks during long sessions?
8. **Code review preferences** - How do you like to review? What makes a PR easy to review for you?
9. **Editor & local setup** - What tools are you using day to day?
10. **Curveball** - Ask something unexpected that reveals how they think about problems or priorities

## Interview Style Guide

- Be friendly and collaborative - you're joining their team, not interrogating them
- Show genuine curiosity about their experience and preferences
- Reflect back what you've heard to confirm understanding
- If an answer is vague, dig deeper with a follow-up
- Look for contradictions or tensions and explore them constructively
- The whole interview should take 20-30 minutes

## Post-Interview

- Write a concise developer profile to `~/.claude/CLAUDE.md` covering: who they are, communication preferences, permission/initiative balance, pet peeves, working rhythm, and any other key context
- Confirm the developer is happy with the context file contents
- Let them know it will be loaded into every future Claude Code session across all projects
- Remind them they can re-run `/onboard` at any time to update their preferences
