# HaizhuDesignSkill

> AI-native frontend design engineering skill for distinctive UI/UX and production-ready React implementation.

## v0.6 — Runtime-first design orchestration

HaizhuDesignSkill is now a **design decision + resource routing + implementation QA system**, not a component catalog. It first understands the product problem, establishes a design system, routes only the tools that are relevant, compiles references into project-native instructions, and then validates the implementation with a repair loop.

## Core toolchain

| Layer | Tool | Responsibility |
|---|---|---|
| Visual direction | Taste Skill | Art direction, hierarchy, anti-slop constraints |
| UX/UI reasoning | UI UX Pro Max | UX patterns, page structure, design-system decisions |
| Design specification | Design MD Collection | Structured design references and implementation guidance |
| Quality refinement | Impeccable | Visual, UX, responsive, accessibility and polish audit |
| Implementation | shadcn | Accessible, composable, source-owned primitives |

Supporting resources are selected only when the UI problem warrants them:

- **Motion Sites** — motion vocabulary and interaction choreography
- **React Bits** — animated React components and backgrounds
- **Uiverse** — lightweight UI element patterns
- **Anime.js** — fine-grained JavaScript animation timelines
- **Aceternity UI** — high-impact animated React patterns

## Architecture

```text
User brief
    ↓
Intent + constraints
    ↓
Design decisions
Taste + UI UX Pro Max + Design MD
    ↓
UX / visual audit
Impeccable
    ↓
Tokens + component architecture
shadcn + project primitives
    ↓
Semantic resource routing
    ↓
Prompt compilation
    ↓
Responsive + motion decisions
    ↓
React / Next.js implementation
    ↓
QA rubric
    ↓
Defect ranking → repair loop → acceptance
```

## What changed in v0.6

### 1. Runtime-first orchestration
The runtime is now the center of the workflow. Adapters provide expertise; the runtime decides when that expertise is relevant.

### 2. Minimal routing
Tool selection is driven by the actual UI problem. The skill explicitly avoids calling or stacking libraries merely because they are available.

### 3. Semantic prompt compilation
External references are converted into intent, target, behavior, trigger, timing/easing, responsive rule, accessibility fallback, and implementation preference instead of copying source or prompt catalogs.

### 4. Repair-oriented QA
The final result is scored across UX, visual coherence, system quality, accessibility, responsiveness, interaction, motion, and performance. Failures are ranked and repaired by impact.

### 5. Anti-slop guardrails
The skill rejects generic decoration as a substitute for design: excessive gradients, glass cards, glows, arbitrary rounding, gratuitous animation, and visually impressive components with weak semantic fit.

## Design principle

**Design system first, components second.**

A component library must serve the product's visual identity, not define it. Establish typography, spacing, color, surfaces, hierarchy, interaction rules, responsive behavior, and motion principles before selecting advanced components.

## Resource routing

Use semantic matching rather than catalog dumping. Normally select only 1–3 references for a single UI problem.

| Problem | First choice | Optional companion |
|---|---|---|
| Visual direction | Taste Skill | Design MD Collection |
| UX architecture | UI UX Pro Max | Impeccable |
| Visual polish | Impeccable | Taste Skill |
| Standard controls | shadcn | UI UX Pro Max |
| Hero motion | Motion Sites | Aceternity UI / React Bits |
| Scroll reveal | Motion Sites | React Bits / Anime.js |
| Magnetic interaction | React Bits | Anime.js |
| Small UI element | Uiverse | shadcn |
| Complex timeline | Anime.js | React Bits |
| High-impact showcase | Aceternity UI | React Bits |

See [`references/routing-matrix.md`](./references/routing-matrix.md) and [`references/adapter-routing.md`](./references/adapter-routing.md).

## Quality gate

A task is not complete merely because the page renders. Check:

- primary task and hierarchy
- visual coherence and anti-slop quality
- responsive behavior
- keyboard/focus/contrast accessibility
- loading/empty/error/disabled/success states
- reduced-motion behavior
- dependency and runtime cost
- component consistency and maintainability

See [`references/evaluation-rubric.md`](./references/evaluation-rubric.md) and [`runtime/qa-engine.md`](./runtime/qa-engine.md).

## Workflows

Built-in guidance covers landing pages, SaaS dashboards, AI products, creative portfolios, and existing UI redesigns.

See [`references/workflows.md`](./references/workflows.md).

## Installation

Copy `SKILL.md` into the skill directory supported by your coding agent, or adapt the package to the agent's skill format.

## Version

**v0.6.0 — Runtime-First Design Orchestration**
