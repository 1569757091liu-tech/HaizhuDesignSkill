# HaizhuDesignSkill

> AI-native frontend design engineering skill for distinctive UI/UX and production-ready React implementation.

## What it is

HaizhuDesignSkill is a routing-and-execution skill for frontend design work. It separates **design judgment**, **UX reasoning**, **implementation primitives**, and **advanced visual references** so an agent does not blindly combine component libraries.

## Core toolchain

| Layer | Tool | Responsibility |
|---|---|---|
| Visual direction | Taste Skill | Art direction, hierarchy, anti-slop constraints |
| UX/UI reasoning | UI UX Pro Max | UX patterns, page structure, design-system decisions |
| Design specification | Design MD Collection | Structured design references and implementation guidance |
| Quality refinement | Impeccable | Visual, UX, responsive, accessibility and polish audit |
| Implementation | shadcn | Accessible, composable, source-owned primitives |

The primary toolchain is complemented by a relevance-matched resource layer:

- **Motion Sites** — motion vocabulary and interaction choreography
- **React Bits** — animated React components and backgrounds
- **Uiverse** — lightweight UI element patterns
- **Anime.js** — fine-grained JavaScript animation timelines
- **Aceternity UI** — high-impact animated React patterns

React Bits describes itself as a collection of customizable animated React components and backgrounds, while shadcn/ui provides source-owned primitives that can be added directly into a project. citeturn0search0turn0search5

## Architecture

```text
User request
    ↓
Brief extraction
    ↓
Design direction
Taste Skill + UI UX Pro Max + Design MD Collection
    ↓
UX / visual audit
Impeccable
    ↓
Design tokens + component architecture
    ↓
Implementation primitives
shadcn + existing project primitives
    ↓
Semantic resource routing
    ├── Motion Sites
    ├── React Bits
    ├── Uiverse
    ├── Anime.js
    └── Aceternity UI
    ↓
React / Next.js implementation
    ↓
Responsive + accessibility + motion QA
```

## The key principle

**Design system first, components second.**

A component library must serve the product's visual identity, not define it. The skill therefore establishes typography, spacing, color, surfaces, hierarchy, interaction rules, responsive behavior, and motion principles before choosing advanced components.

## Resource routing

The skill uses semantic matching rather than catalog dumping.

Examples:

- Hero motion → Motion Sites → Aceternity UI / React Bits
- Scroll reveal → Motion Sites → React Bits / Anime.js
- Magnetic interaction → React Bits → Anime.js
- Small UI element → Uiverse → shadcn
- Standard form/dialog/table → shadcn
- Complex timeline choreography → Anime.js
- Visual redesign → Taste Skill → Impeccable
- UX-heavy product flow → UI UX Pro Max → Impeccable

Each candidate is scored for semantic fit, visual fit, implementation fit, performance fit, and accessibility fit. Normally only 1–3 references are selected for a single UI problem.

See [`references/routing-matrix.md`](./references/routing-matrix.md).

## Workflows

Built-in workflow guidance covers:

- Landing pages
- SaaS dashboards
- AI products
- Creative portfolios
- Existing UI redesigns

See [`references/workflows.md`](./references/workflows.md).

## Prompt engineering layer

The skill converts external references into **semantic implementation prompts** rather than copying large prompt libraries or source files.

Every extracted reference can be expressed as:

```text
intent
→ target element
→ visual behavior
→ interaction trigger
→ timing/easing
→ responsive rule
→ accessibility fallback
→ implementation preference
```

Reusable templates are available in [`references/prompt-templates.md`](./references/prompt-templates.md).

## Quality gate

Before completion, the skill checks:

- visual hierarchy
- UX clarity
- responsive behavior
- accessibility and keyboard support
- interaction states
- reduced-motion behavior
- performance and dependency cost
- component consistency
- anti-slop quality

See [`references/qa-checklist.md`](./references/qa-checklist.md).

## Installation

Copy `SKILL.md` into the skill directory supported by your coding agent, or adapt the package to the agent's skill format.

## Version

**v0.2.0 — Design Engineering Router**
