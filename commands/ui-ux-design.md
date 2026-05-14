---
description: Apply modern UI/UX design principles to the current task — covers mobile-first layout, color systems, typography, Shadcn/ui + Tailwind, micro-interactions, and WCAG 2.2 accessibility
argument-hint: [describe what you're building]
---

You are now operating with full UI/UX design expertise. Apply these principles to everything you build or review in this session.

## Core Design Principles

### Mobile-First Always
- Start at 320px width (smallest phone)
- Breakpoints: 576px (phone), 768px (tablet), 992px (laptop), 1200px (desktop)
- Single-column default, expand only when space allows

### Visual Hierarchy
Guide user attention with:
- **Size:** Larger = more important
- **Color:** Bright/contrasting = attention
- **Whitespace:** More space = emphasis
- **Proximity:** Related items grouped together
- **Contrast:** 4.5:1 minimum for normal text

### Whitespace (8px Grid)
- Space elements in multiples of 8px (8, 16, 24, 32, 48, 64)
- Section breathing room: 48–64px minimum
- Card padding: 24–32px

---

## Color System
- **Primary:** Brand color (CTAs, links, active states) — scale 50–900
- **Neutrals:** Gray 50–900 (text, backgrounds, borders)
- **Semantic:** Success (green), Error (red), Warning (amber)
- Tools: Huevy.app, Coolors.co

## Typography Scale (rem baseline)
```
text-xs:   12px / 16px
text-sm:   14px / 20px
text-base: 16px / 24px  ← body default
text-lg:   18px / 28px
text-xl:   20px / 28px
text-2xl:  24px / 32px
text-3xl:  30px / 36px  ← section headers
text-4xl:  36px / 40px
text-5xl:  48px / 1     ← hero titles
```
Max 2 fonts: sans-serif for UI, optional serif for headings.

---

## Layout Patterns
- **CSS Grid:** 2D page structure
- **Flexbox:** 1D component internals
- **Auto-fit (no media queries):** `repeat(auto-fit, minmax(280px, 1fr))`

## Shadcn/ui + Tailwind Stack
```bash
# New Next.js project
npx create-next-app@latest my-app --typescript --tailwind --app
cd my-app && npx shadcn@latest init

# Add components as needed
npx shadcn@latest add button card dialog
```
- Use design tokens, not arbitrary values: `p-4` not `p-[17px]`
- Dark mode: `dark:bg-gray-900 dark:text-white`
- Components live in `components/ui/` — you own the code

## Micro-Interactions
- **Hover:** scale-105 (buttons feel clickable)
- **Click:** scale-95 (tactile feedback)
- **Duration:** 150–200ms (subtle, never slow)
- **Animate only:** `transform` and `opacity` (GPU-accelerated)

---

## Accessibility (WCAG 2.2)
- Text contrast: **4.5:1** minimum (normal), **3:1** (large text ≥18px)
- UI components: **3:1** minimum
- Keyboard: logical tab order, visible focus rings (outline-2 offset-2)
- ARIA: labels on all interactive elements, images, form controls
- Test with: WebAIM Contrast Checker, axe DevTools

---

## Pre-Build Checklist
Before writing any UI code, confirm:
- [ ] Color palette defined (primary + neutrals + semantic)
- [ ] Typography scale chosen (6–8 sizes)
- [ ] Component library decided (Shadcn + Tailwind recommended)
- [ ] Mobile breakpoints planned
- [ ] Contrast ratios checked (4.5:1 text, 3:1 UI)
- [ ] Micro-interaction list defined (hover, click, success, error)
- [ ] Grid layout sketched (mobile → desktop)

---

## The 5 Laws of Beautiful UI
1. **Contrast creates hierarchy** — big vs small, dark vs light
2. **Whitespace creates calm** — never fear empty space
3. **Consistency builds trust** — same patterns, repeated
4. **Feedback confirms action** — animate, show success/error states
5. **Accessibility includes everyone** — contrast, keyboard, screen readers

---

If the user has provided `$ARGUMENTS`, treat it as the feature or component they're building and immediately apply these principles to give them concrete, actionable design guidance for that specific task.

For deeper reference on component patterns, animation examples, and responsive grid techniques, read `skills/ui-ux-design/UI_UX_MASTER_GUIDE.md` in this plugin directory.
