# Skills glossary

## What are skills?

Skills are domain-specific knowledge files that commands and agents reference for methodology, quality standards, and structured workflows. They don't run on their own — they give the AI deeper expertise when a command points to them.

## How they work

- A command references a skill in its Persona or task steps (e.g. "Follow `.cursor/skills/presentation.md`")
- The AI reads the skill file at runtime and applies the methodology
- Skills define **what to do and how**, commands define **when and with what input**
- One skill can be referenced by multiple commands

## All skills

| Skill | Used by | Description |
|-------|---------|-------------|
| `presentation` | `/create-presentation` | Kapterev dramaturgy method — dramatic structure, slide content rules, speaker notes, and quality checklist for presentations. |

## Skills vs commands

| Use **skills** when... | Use **commands** when... |
|---|---|
| Defining reusable methodology or domain knowledge | Defining a user-facing workflow with input/output |
| The same expertise applies across multiple commands | The task is a single, self-contained action |
| You need detailed quality standards or checklists | You need a persona, mode, and structured steps |

## Creating a new skill

Add a markdown file to `.cursor/skills/` with YAML frontmatter:

```markdown
---
name: skill-name
description: What this skill covers and when to use it.
---

# Skill Name

## When to use this skill
Trigger conditions.

## Step 1 — ...
...

## Step N — ...
...

## Quality checklist
- [ ] ...
```

Best practices:
- Keep skills focused on one domain — don't combine presentation advice with copywriting rules
- Include a quality checklist at the end so commands can validate output
- Write steps as methodology, not as user-facing instructions
- Reference skills from commands explicitly — skills don't auto-activate
