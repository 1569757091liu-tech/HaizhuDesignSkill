---
name: haizhu-design-skill
description: A design-engineering skill for building distinctive, production-ready frontend interfaces. It orchestrates Taste Skill, Impeccable, shadcn, UI UX Pro Max, and Design MD Collection, then routes relevant motion/UI references from Motion Sites, React Bits, Uiverse, Anime.js, and Aceternity UI. Use when the user asks to design, redesign, prototype, implement, polish, animate, or review a web UI/frontend.
---

# Haizhu Design Skill

## Mission

Turn an ambiguous frontend request into a coherent design direction, implementable UI system, and production-oriented React/Next.js code. Avoid generic AI-generated UI. Prefer a small number of strong visual decisions over decorative effects.

## Runtime-first architecture

```text
User brief
  ↓
Intent + constraints
  ↓
Design decision engine
  ├─ Taste
  ├─ UI UX Pro Max
  └─ Design MD
  ↓
UX / visual audit
  └─ Impeccable
  ↓
System + component mapping
  └─ shadcn / project primitives
  ↓
Problem-specific resource router
  ├─ Motion Sites
  ├─ React Bits
  ├─ Uiverse
  ├─ Anime.js
  └─ Aceternity UI
  ↓
Prompt compiler + implementation plan
  ↓
Responsive + motion decisions
  ↓
Implementation
  ↓
QA + repair loop
```

Runtime contracts live in `runtime/`. Adapter contracts live in `adapters/`. Routing guidance lives in `references/`.

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

For every request:

1. Extract intent, constraints, existing stack, and acceptance criteria.
2. Classify the problem as visual, UX, structure, component, motion, responsive, or polish.
3. Select the minimum core adapters needed.
4. Select supporting adapters only for unresolved problems.
5. Score candidates from 0–3 for semantic, visual, implementation, performance, and accessibility fit.
6. Reject candidates below the threshold or those that introduce unnecessary complexity.
7. Compile selected references into project-native instructions.
8. Implement using existing project primitives before adding dependencies.
9. Run the QA gate and repair the highest-impact failures first.

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
- explicit non-goals

Infer conservatively when non-critical information is missing. Do not invent brand requirements.

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

Produce decisions before component selection.

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

### Phase 7 — Quality gate + repair loop

Evaluate five dimensions: UX clarity, visual coherence, implementation quality, accessibility, and performance. Record failures as concrete defects, rank them by impact, repair the top issues, then re-run the gate.

A task is not complete merely because the page renders. It is complete when the primary task is clear, the system is coherent, critical states work, responsive behavior is intentional, and motion does not create accessibility or performance regressions.

See `runtime/qa-engine.md` and `references/evaluation-rubric.md`.

## Anti-slop rules

Reject or simplify patterns that are generic by default:
- excessive gradient backgrounds
- repeated glass cards without semantic need
- oversized hero typography without hierarchy
- decorative blobs/glows competing with content
- animation on every element
- arbitrary rounded corners and shadows
- icon-only actions without accessible names
- duplicated component variants with no behavioral difference

A distinctive interface should come from composition, typography, spacing, color, content hierarchy, and intentional interaction—not from piling on effects.

## Motion rules

Motion must have a job:
- **Orientation** — establishes context or hierarchy.
- **Feedback** — confirms an action/state change.
- **Continuity** — connects related states.
- **Emphasis** — directs attention.
- **Atmosphere** — optional and sparse.

Prefer subtle, composable motion. Avoid stacking parallax + cursor effects + glow + blur + text animation in one viewport unless the brief explicitly calls for an experimental showcase. Respect `prefers-reduced-motion` and preserve task completion without animation.

## Output contract

For a design/implementation plan return:
1. Design direction
2. UX structure
3. Component/system map
4. Selected adapters/references and why
5. Motion plan
6. Responsive plan
7. Implementation plan
8. QA risks and acceptance criteria

When implementing directly, keep reasoning compact and prioritize working code.

## Hard constraints

- Design system first, components second.
- Never let a component library determine visual identity.
- Never add animation without a purpose.
- Preserve accessibility and reduced-motion behavior.
- Prefer existing project dependencies over new ones.
- Adapt external references instead of blindly copying them.
- Optimize for the final interface, not the number of tools called.
