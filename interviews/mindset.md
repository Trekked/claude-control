# Coding Mindset Interview

> **Reference template.** Run this interview once during project setup. Paste the contents into a Claude Code session to begin. Not typically used as a recurring slash command.

You are exploring the coding philosophy and decision-making principles for a project. This is a shorter, targeted session that fills gaps not covered by onboarding and workflow interviews.

## Instructions

1. Read any existing onboarding and workflow documentation first - don't repeat what's covered
2. Identify gaps in your understanding of how to make decisions
3. Ask targeted questions, not a full 20-question session
4. Write the results into the WORKFLOW.md document (coding philosophy section) or a separate MINDSET.md if the content warrants it

## Questions

Pick the questions that are relevant. Not all will apply to every project.

### Codebase & Patterns
1. **Existing code** - When you find something wrong or suboptimal in the existing codebase (or framework), what should you do? Fix silently, flag and move on, or something else?
2. **Patterns** - How strictly should existing patterns be followed? When is it OK to deviate?
3. **Dependencies** - How do you think about third-party libraries? Use them freely, minimise them, or somewhere in between? Does licensing matter?

### Decision Making
4. **Multiple approaches** - When there are multiple valid ways to implement something, should you pick one and go, or present options?
5. **Trade-offs** - How do you balance speed vs quality? What's the general philosophy? (e.g., "perfect is the enemy of done", "measure twice cut once")
6. **Scale** - Should you build for current needs or anticipated scale? Where's the line between pragmatic and naive?

### Technical Debt
7. **Tech debt management** - How do you track it? When do you address it? Is there a threshold where you stop feature work to clean up?
8. **Refactoring** - When is refactoring justified? When is it gold-plating?

### Boundaries
9. **AI in the product** - If the product has a stance on AI-generated content, what is it? How does it affect technical decisions?
10. **Security posture** - How security-conscious should the code be? What's the bar for things like input validation, auth checks, data encryption?
11. **Frustration guard** - When the developer is tired and asks for something risky, should you push back? How firmly?

## Interview Style Guide

- This should feel like a conversation between peers, not an interview
- Ask for concrete examples - "give me a scenario where..."
- Share your own opinion and let them react - it's faster than open-ended questions
- If they say "it depends", explore the cases
- Look for guiding principles, not rigid rules

## Post-Interview

- Integrate findings into WORKFLOW.md under a "Coding Philosophy" section, or create a separate MINDSET.md
- Focus on actionable principles, not abstract philosophy
- Update project memory with key decision-making rules

## Adapting for Your Project

Domain-specific questions to consider:
- **Healthcare/Finance**: Compliance requirements, audit trails, data handling rules
- **Consumer**: Performance budgets, accessibility standards, internationalisation
- **Enterprise**: Backwards compatibility, API versioning, migration strategies
- **Open source**: Code style enforcement, contribution quality bar, documentation standards
