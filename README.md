# NG Web Designs

Shared project for NG Web Designs. It includes the Claude Code skills we use for design work, so everyone who clones the repo gets the same setup.

## What are skills?

A skill is a folder of instructions (and sometimes scripts or data) that teaches Claude Code how to handle a specific kind of task. Each skill has a `SKILL.md` file with a name, a short description, and the instructions.

You don't need to call skills by hand. Claude reads each skill's description and uses it automatically when your request matches. You can also run one directly by typing `/` followed by its name, for example `/frontend-design`.

Skills in this repo live in `.claude/skills/`, so they're available whenever you open this project in Claude Code.

## Included skills

### frontend-design

Guidance for creating distinctive, intentional visual designs instead of generic, template-looking pages.

- Picks a clear visual direction based on the subject and audience
- Chooses typefaces, color palettes and layouts on purpose
- Avoids common "AI-generated" looks (cream backgrounds with terracotta accents, identical rounded cards, all-caps labels, etc.)
- Plans the design first, checks it against the brief, then builds it
- Covers accessibility, responsive layout, motion and interface copy

Source: [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/frontend-design)

### ui-ux-pro-max

A searchable UI/UX knowledge base for web, mobile and desktop interfaces.

- Styles, product color palettes, font pairings, icons, chart types and UX guidelines
- Advice for specific stacks (React, Next.js, Vue, Tailwind, Flutter, SwiftUI and more)
- Prioritized checks: accessibility, touch targets, performance, layout, typography, animation, forms, navigation
- Can generate a full design system for a project

Source: [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)

**Requires Python 3** for its search scripts. Check with `python --version` (or `python3 --version`).

## Getting started

1. Install [Claude Code](https://claude.com/claude-code).
2. Clone this repo:
   ```bash
   git clone https://github.com/Giorgosskep/webdesignsNG.git
   ```
3. Open the `webdesignsNG` folder in Claude Code.
4. Ask for design work, for example:
   - "Build a landing page for a local bakery"
   - "Review this page for accessibility and UX problems"
   - "Suggest a color palette and fonts for a law firm website"

## Adding or updating skills

- **Add a skill:** put its folder (containing `SKILL.md`) in `.claude/skills/`, then commit and push.
- **Update a skill:** replace its folder with the newer version, then commit and push.
- **Remove a skill:** delete its folder, then commit and push.

Start a new Claude Code session to pick up changes.

## Project structure

```
.
├── .claude/
│   └── skills/
│       ├── frontend-design/   # Visual design guidance
│       └── ui-ux-pro-max/     # UI/UX knowledge base + search scripts
├── .gitattributes             # Line-ending rules
├── .gitignore
└── README.md
```
