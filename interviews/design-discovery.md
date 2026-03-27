# Design Discovery Interview

> **Reference template.** Run this interview once during project setup via the `/interviews` command. Not typically used as a recurring slash command.

You are establishing the visual and UI design principles for a project. The goal is to capture enough design direction that agents can build UI without constant back-and-forth on aesthetic decisions.

## Instructions

1. Read any existing project documentation (PRODUCT, WORKFLOW, etc.) for context
2. Conduct a conversational interview covering the topics below
3. Ask one question at a time, follow up on specifics
4. If the developer has reference sites, screenshots, or mockups, ask to see them
5. Write the results to two places:
   - **Transcript**: A file with verbatim Q&A (ask where to save)
   - **Synthesised document**: A `DESIGN.md` reference document for UI work

## Questions

### Existing Assets (Q1)
1. **Existing assets** - Do you already have a logo, brand guide, colour palette, fonts, icon set, or any other design assets? (If yes, review them before continuing - they may answer several questions below.)

### Typography & Colour (Q2-4)
2. **Typography** - Do you have fonts in mind? Serif, sans-serif, monospace? What feeling should the type convey? (professional, playful, editorial, etc.)
3. **Colour palette** - Any brand colours? Dark mode, light mode, or both? What's the general mood? (bold, muted, earthy, neon, etc.)
4. **References** - Show me 2-3 websites or apps whose visual style you admire. What specifically do you like about each?

### Layout & Components (Q5-7)
5. **Layout philosophy** - Full-bleed or contained? Dense or spacious? Card-heavy or minimal? How much whitespace?
6. **Component style** - Rounded or sharp corners? Borders or shadows? Flat or layered? Translucent or solid?
7. **Responsive approach** - Mobile-first or desktop-first? What's the primary device for your users?

### Brand & Tone (Q8-9)
8. **Visual personality** - If this product were a person, how would they dress? (casual, outdoorsy, minimalist, maximalist, etc.)
9. **What to avoid** - Are there design styles or patterns you actively dislike? Things that would feel wrong for this product?

### Practical (Q10)
10. **Accessibility** - What's the accessibility bar? WCAG AA, AAA, or "do your best"? Any specific requirements?

## Interview Style Guide

- Show genuine interest in their aesthetic preferences - this is personal
- When they say "clean" or "modern", dig deeper - those words mean different things to different people
- Ask for examples over descriptions - "show me what you mean" beats "describe what you want"
- It's OK if they don't know - capture what they do know and note the gaps
- This should be quick and focused - 15-20 minutes

## Post-Interview

- Write a synthesised `DESIGN.md` covering: typography, colour, layout, components, accessibility, and any brand guidelines
- Keep it practical and actionable - agents should be able to reference it during UI work
- Include links to reference sites if mentioned
- Note areas that are undecided with a clear "TBD" marker
- Update project memory with key design decisions
- Ask the developer to review and refine

## Adapting for Your Project

Consider adding questions for:
- **Consumer app**: Onboarding flow style, empty states, micro-interactions
- **B2B/Dashboard**: Data density, table design, chart preferences
- **Content platform**: Reading experience, typography scale, media handling
- **E-commerce**: Product display, checkout flow, trust signals
