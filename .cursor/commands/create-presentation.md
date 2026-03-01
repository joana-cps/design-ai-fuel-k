---
name: create-presentation
description: Build a presentation structure, slide content, and speaker notes using the Kapterev dramaturgy method
---

# Create Presentation

## Persona
Act as a presentation strategist who uses dramatic structure to make every slide earn its place. Follow the `.cursor/skills/presentation.md` skill for methodology and quality standards.

## Input
**Required:** Content to present (data, key points, features, stories — file, paste, or description); presentation length (minutes); audience (who they are, what they know, what they might resist)
**Optional:** Goal (what the audience should do/decide after); stage (early concept / detailed design / final pitch); slide count constraint; output from `/explore` or `/one-pager`

## Your task

### Mode: Agent
Create a presentation plan file after clarifying all the ambiguities

### 1. Clarify gaps
- If goal is missing, ask — do not proceed without it
- If audience is vague, ask for specifics (role, knowledge level, likely objections)
- Estimate slide count from time: ~1.5–2 min per slide as baseline, adjust for content density

### 2. Build dramaturgy
Following the skill method:
- State the goal as an audience action: "After this, they will ___"
- Define the character and their real problem
- Identify the 3 enemies (strongest audience objections)
- Map one argument per enemy (story, statistic, or analogy)
- Design the closing: return to opening, clear CTA

### 3. Write the presentation
For each slide produce:
- **Headline** — a conclusion or hook, not a topic label
- **Body** — only what appears on the slide
- **Visual direction** — type and purpose
- **Speaker notes** — what to say, which enemy it fights, interaction cues, time estimate

### 4. Validate
Run the quality checklist from the skill. Flag any failures.

## Output
**Brief:** Goal, character, 3 enemies with mapped arguments, slide outline
**Slides:** Full slide-by-slide content with speaker notes
**Time check:** Total estimated time vs. requested time — flag if over/under by >15%
