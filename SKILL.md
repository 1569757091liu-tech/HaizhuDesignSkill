---
name: haizhu-design-skill
description: A design-engineering skill for building distinctive, production-ready frontend interfaces. It orchestrates Taste Skill, Impeccable, shadcn, UI UX Pro Max, and Design MD Collection, then routes relevant motion/UI references from Motion Sites, React Bits, Uiverse, Anime.js, and Aceternity UI. Use when the user asks to design, redesign, prototype, implement, polish, animate, or review a web UI/frontend.
---

# Haizhu Design Skill

## Mission

Turn an ambiguous frontend request into a coherent design direction, implementable UI system, and production-oriented React/Next.js code. Avoid generic AI-generated UI. Prefer a small number of strong visual decisions over decorative effects.

## Architecture

```text
User brief
  ↓
Brief classifier
  ↓
Core design adapters
  ├─ Taste
  ├─ UI UX Pro Max
  ├─ Design MD
  ├─ Impeccable
  └─ shadcn
  ↓
Problem classification
  ↓
Supporting resource router
  ├─ Motion Sites
  ├─ React Bits
  ├─ Uiverse
  ├─ Anime.js
  └─ Aceternity UI
  ↓
Semantic prompt extraction
  ↓
Project-native implementation
  ↓
QA + refinement
```

Adapter contracts live in `adapters/`. Routing guidance lives in `references/adapter-routing.md`.

## Core adapters

### Taste Skill
Establish visual direction, anti-slop constraints, hierarchy, typography, spacing, color, surface language, and motion taste.

### UI UX Pro Max
Solve product UX, information architecture, page patterns, interaction models, responsive strategy, and design-system decisions.

### Design MD Collection
Turn visual intent into structured specifications: tokens, page anatomy, components, states, responsive rules, and implementation notes.

### Impeccable
Audit and refine the result. Prioritize fixes by user impact rather than redesigning everything.

### shadcn
Translate approved decisions into accessible, composable, project-owned primitives. Component defaults must not determine the product identity.

## Supporting resource adapters

Use only when the current UI problem warrants them.

- **Motion Sites** → motion language and choreography.
- **React Bits** → React-native animated component patterns.
- **Uiverse** → small UI elements and micro-interactions.
- **Anime.js** → precise JavaScript timelines and coordinated sequences.
- **Aceternity UI** → high-impact animated React patterns for focal/showcase surfaces.

## Adapter selection protocol

For every request, classify the problem before selecting a resource.

1. Identify the user's primary goal.
2. Determine whether the problem is visual, UX, structural, component-level, motion, or polish.
3. Select the minimum core adapters needed.
4. Select supporting adapters only for unresolved UI problems.
5. Score candidates from 0–3 for semantic, visual, implementation, performance, and accessibility fit.
6. Keep the smallest set that sufficiently solves the problem.
7. Translate external references into project-native guidance.
8. Reject references that conflict with the design system, accessibility, performance, or product goal.

Never select a resource solely because the user mentioned its library.

## Execution protocol

### Phase 0 — Understand the brief

Extract:
- product/page type
- target users and primary task
- content hierarchy
- required sections/components
- brand/style references
- technical stack and existing codebase
- responsive requirements
- interaction/motion requirements
- accessibility/performance constraints

Infer conservatively when non-critical information is missing.

### Phase 1 — Establish design direction

Use Taste + UI UX Pro Max + Design MD responsibilities to define:
- visual concept
- typography roles
- color strategy
- spacing rhythm
- surface/elevation strategy
- layout grid
- component language
- interaction principles
- motion principles
- responsive behavior
- anti-patterns to avoid

Do not start by selecting random components.

### Phase 2 — UX and visual audit

Use Impeccable-style questions:
- Is the primary action obvious?
- Does hierarchy survive a 3-second scan?
- Are density and whitespace intentional?
- Are typography and contrast legible?
- Are repeated patterns consistent?
- Does the design work at mobile/tablet/desktop widths?
- Are loading, empty, error, disabled, hover, focus, and success states covered?
- Does motion communicate state or hierarchy rather than decoration?

### Phase 3 — Build the system

Use shadcn principles:
- accessible primitives
- project-owned components
- design tokens/CSS variables
- composition over one-off markup
- keyboard/focus behavior
- minimal dependencies

Map decisions into tokens → primitives → composed components → sections → templates.

### Phase 4 — Resource routing

| Need | Primary | Secondary |
|---|---|---|
| Hero motion | Motion Sites | Aceternity UI / React Bits |
| Scroll choreography | Motion Sites | React Bits / Anime.js |
| Magnetic/cursor interaction | React Bits | Anime.js |
| Micro UI element | Uiverse | shadcn |
| High-impact landing effect | Aceternity UI | React Bits |
| Complex timeline | Anime.js | React Bits |
| Standard form/dialog/table | shadcn | UI UX Pro Max |
| Visual redesign | Taste | Impeccable |
| UX-heavy product flow | UI UX Pro Max | Impeccable |

### Phase 5 — Extract semantic prompts

For every selected external reference, output only:
- intent
- target element
- visual behavior
- interaction trigger
- timing/easing
- responsive rule
- accessibility fallback
- implementation preference

Do not reproduce large portions of third-party source code or proprietary prompt collections.

Example:

> Use a restrained spotlight interaction for the hero card. Pointer proximity subtly shifts a low-opacity radial highlight while content remains stable. Disable the effect under `prefers-reduced-motion`. Prefer CSS variables or a lightweight pointer handler over a new animation dependency.

### Phase 6 — Implement

Default target:
- React + TypeScript
- Next.js when indicated
- Tailwind CSS when already present
- shadcn/ui when appropriate

Priority:
1. semantic structure
2. responsive layout
3. accessibility
4. visual hierarchy
5. interaction states
6. motion
7. micro-polish

### Phase 7 — Quality gate

Verify:
- no generic/template-looking sections unless requested
- no excessive gradients/glows/cards
- no gratuitous animation
- no broken responsive layout
- no inaccessible contrast or focus states
- no missing product states
- no animation that blocks task completion
- reduced-motion behavior exists where motion is meaningful
- sensible component reuse
- maintainable code

## Motion rules

Motion must have a job:
- **Orientation** — establishes context or hierarchy.
- **Feedback** — confirms an action/state change.
- **Continuity** — connects related states.
- **Emphasis** — directs attention.
- **Atmosphere** — optional and sparse.

Prefer subtle, composable motion. Avoid stacking parallax + cursor effects + glow + blur + text animation in one viewport unless the brief explicitly calls for an experimental showcase.

## Output contract

For a design/implementation plan return:
1. Design direction
2. UX structure
3. Component/system map
4. Selected adapters/references and why
5. Motion plan
6. Implementation plan
7. Quality checklist

When implementing directly, keep reasoning compact and prioritize working code.

## Hard constraints

- Design system first, components second.
- Never let a component library determine visual identity.
- Never add animation without a purpose.
- Preserve accessibility and reduced-motion behavior.
- Prefer existing project dependencies over new ones.
- Adapt external references instead of blindly copying them.
