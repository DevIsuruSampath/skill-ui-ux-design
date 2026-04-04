# UI/UX Design Skill

A plugin that provides modern UI/UX design principles, patterns, and best practices for web and mobile applications.

## When to Use

Activate this skill when:

- Building or designing web/mobile interfaces
- Choosing colors, typography, or layout systems
- Implementing responsive design (mobile-first)
- Ensuring accessibility compliance (WCAG 2.2)
- Setting up Shadcn/ui + Tailwind CSS projects
- Creating micro-interactions and animations
- Reviewing UI/UX decisions before coding

## What's Included

- **Core Design Principles** - Mobile-first approach, visual hierarchy, whitespace, typography
- **Color & Typography Systems** - Scales, pairings, and 8px baseline grid
- **Layout Patterns** - CSS Grid, Flexbox, auto-fit responsive layouts
- **Shadcn/ui + Tailwind Stack** - Setup, component patterns, best practices
- **Micro-Interactions** - Hover, click, and transition guidelines
- **Accessibility (WCAG 2.2)** - Contrast ratios, keyboard nav, ARIA labels
- **2026 Design Trends** - Current patterns and inspiration sources

## Installation

### Option 1: Install as a Claude Code Skill (Recommended)

Clone this repo into your local skills directory:

```bash
# Create skills directory if it doesn't exist
mkdir -p ~/.claude/skills

# Clone the skill
git clone https://github.com/DevIsuruSampath/skill-ui-ux-design.git ~/.claude/skills/ui-ux-design
```

Restart Claude Code. The skill will be automatically available when you ask about UI/UX topics.

### Option 2: Install via CLAUDE.md

Add a reference in your project's `CLAUDE.md`:

```bash
# Clone to any location
git clone https://github.com/DevIsuruSampath/skill-ui-ux-design.git

# Add to CLAUDE.md
echo "- Read @skill-ui-ux-design/SKILL.md when doing UI/UX work" >> CLAUDE.md
```

### Option 3: Manual Install

Copy the files into your project and reference `SKILL.md` in your `CLAUDE.md` or agent instructions.

## File Structure

```
├── _meta.json                 # Skill metadata (slug, version, owner)
├── SKILL.md                   # Skill entry point and quick reference
├── UI_UX_MASTER_GUIDE.md      # Comprehensive design reference
└── references/
    ├── ACCESSIBILITY.md       # WCAG 2.2 compliance guide
    ├── COMPONENTS.md          # Shadcn/ui + Tailwind component patterns
    └── DESIGN_SYSTEM.md       # Full design system reference
```

## Version

1.0.0
