# UI/UX Design Plugin

A Claude Code plugin that provides modern UI/UX design principles, patterns, and best practices for web and mobile applications.

## What's Included

- `/ui-ux-design` slash command — activates full design expertise for the current session
- `ui-ux-reviewer` agent — reviews components and pages for design quality and WCAG 2.2 compliance
- **Core Design Principles** — Mobile-first, visual hierarchy, 8px grid, whitespace
- **Color & Typography Systems** — Scales, pairings, semantic colors
- **Layout Patterns** — CSS Grid, Flexbox, auto-fit responsive layouts
- **Shadcn/ui + Tailwind Stack** — Setup, component patterns, best practices
- **Micro-Interactions** — Hover, click, and transition guidelines
- **Accessibility (WCAG 2.2)** — Contrast ratios, keyboard nav, ARIA labels
- **2026 Design Trends** — Current patterns and inspiration sources

## Installation

### Option 1: Local Plugin (Recommended)

Clone this repo into the Claude Code local plugins directory:

```bash
git clone https://github.com/DevIsuruSampath/skill-ui-ux-design.git \
  ~/.claude/plugins/local/plugins/ui-ux-design
```

Restart Claude Code. The plugin is automatically detected from the local marketplace.

### Option 2: Manual reference via CLAUDE.md

```bash
git clone https://github.com/DevIsuruSampath/skill-ui-ux-design.git
```

Add to your project's `CLAUDE.md`:
```
@skill-ui-ux-design/skills/ui-ux-design/SKILL.md
```

## Usage

After installing, use the slash command in any Claude Code session:

```
/ui-ux-design
```

Or with context:
```
/ui-ux-design building a dashboard with cards and a sidebar
```

To review existing UI code, mention the `ui-ux-reviewer` agent in your prompt.

## File Structure

```
├── .claude-plugin/
│   └── plugin.json              # Plugin manifest
├── commands/
│   └── ui-ux-design.md          # /ui-ux-design slash command
├── agents/
│   └── ui-ux-reviewer.md        # Design review agent
├── skills/ui-ux-design/
│   ├── SKILL.md                 # Quick reference
│   ├── UI_UX_MASTER_GUIDE.md    # Comprehensive design reference
│   └── references/
│       ├── ACCESSIBILITY.md     # WCAG 2.2 compliance guide
│       ├── COMPONENTS.md        # Shadcn/ui + Tailwind patterns
│       └── DESIGN_SYSTEM.md     # Full design system reference
└── README.md
```

## Version

1.0.0
