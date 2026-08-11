---
name: haizhu-design-skill
description: A design-engineering skill for building distinctive, production-ready frontend interfaces. It orchestrates Taste Skill, Impeccable, shadcn, UI UX Pro Max, and Design MD Collection, then selects relevant motion/UI resources from Motion Sites, React Bits, Uiverse, Anime.js, and Aceternity UI. Use when the user asks to design, redesign, prototype, implement, polish, animate, or review a web UI/frontend.
---

# Haizhu Design Skill

## Mission

Turn an ambiguous frontend request into a coherent design direction, an implementable UI system, and production-oriented React/Next.js code. Avoid generic AI-generated UI. Prefer a small number of strong visual decisions over decorative effects.

## Core orchestration

Five design tools form the primary pipeline:

1. **Taste Skill** — establish visual direction, anti-slop constraints, hierarchy, typography, spacing, color, and motion taste.
2. **Impeccable** — audit/refine visual quality, layout, hierarchy, accessibility, responsive behavior, and polish.
3. **shadcn** — provide accessible, composable, source-owned UI primitives and implementation patterns.
4. **UI UX Pro Max** — generate/validate practical UX, UI patterns, design-system decisions, and implementation guidance.
5. **Design MD Collection** — use as a design-spec/reference layer for turning visual intent into structured implementation guidance.

The five tools are complementary, not interchangeable. Do not ask every tool to solve the same problem.

## Resource selection layer

When the user needs advanced interaction, motion, or distinctive components, select only the relevant resources:

- **Motion Sites** → motion language, interaction choreography, scroll/hover/page-transition inspiration, and motion prompt vocabulary.
- **React Bits** → React-native animated components/backgrounds and implementation patterns.
- **Uiverse** → lightweight UI element ideas and interaction variants; adapt rather than blindly copy.
- **Anime.js** → timeline-based or fine-grained JavaScript animation when CSS/React transitions are insufficient.
- **Aceternity UI** → premium-feeling animated React patterns such as hero effects, spotlight/glow, parallax, beams, cards, and scroll reveals.

Use these as a relevance-matched reference layer, not as a requirement to add animation everywhere.

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

If critical information is missing, infer conservatively and state the assumptions internally before implementation.

### Phase 1 — Establish the design direction

Run the conceptual responsibilities of Taste Skill + UI UX Pro Max + Design MD Collection.

Produce a compact design brief containing:
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
- explicit anti-patterns to avoid

Do not start by selecting random components.

### Phase 2 — UX and visual audit

Use Impeccable-style review questions:
- Is the primary action obvious?
- Does hierarchy survive a 3-second scan?
- Are density and whitespace intentional?
- Are typography and contrast legible?
- Are repeated patterns actually consistent?
- Does the design work at mobile/tablet/desktop widths?
- Are states covered: loading, empty, error, disabled, hover, focus, success?
- Does motion communicate state or hierarchy rather than decoration?

### Phase 3 — Build the system

Use shadcn principles for implementation:
- prefer accessible primitives
- keep component ownership in the project
- use design tokens/CSS variables where practical
- compose primitives instead of creating one-off markup
- preserve keyboard/focus behavior
- avoid unnecessary dependencies

Map design decisions into:
- tokens
- primitives
- composed components
- sections
- page templates

### Phase 4 — Select supporting resources

Classify the request before selecting resources.

| Need | Primary resource | Secondary resource |
|---|---|---|
| Hero motion | Motion Sites | Aceternity UI / React Bits |
| Scroll reveal | Motion Sites | React Bits / Anime.js |
| Magnetic/cursor interaction | React Bits | Anime.js |
| Decorative UI element | Uiverse | shadcn |
| High-impact landing-page effect | Aceternity UI | React Bits |
| Complex animation timeline | Anime.js | React Bits |
| Standard form/dialog/table | shadcn | UI UX Pro Max |
| Visual redesign | Taste Skill | Impeccable |
| UX-heavy product flow | UI UX Pro Max | Impeccable |

### Phase 5 — Convert references into prompts

Do not dump a library's entire component catalog into the model context. Extract only the semantic attributes needed for the current task.

For each selected reference, convert it into a **design implementation prompt** with:
- intent
- target element
- visual behavior
- interaction trigger
- timing/easing
- responsive rule
- accessibility fallback
- implementation preference

Example:

> Use a restrained spotlight interaction for the hero card: pointer proximity subtly shifts the radial highlight, opacity remains low, the card content does not move, and `prefers-reduced-motion` disables the effect. Implement with CSS variables or a lightweight React pointer handler; do not add a heavy animation dependency.

This is preferable to copying a component description verbatim.

### Phase 6 — Implement

Default frontend target:
- React + TypeScript
- Next.js when the project indicates it
- Tailwind CSS when already present
- shadcn/ui when appropriate

Implementation priorities:
1. semantic structure
2. responsive layout
3. accessibility
4. visual hierarchy
5. interaction states
6. motion
7. micro-polish

### Phase 7 — Quality gate

Before declaring completion, verify:
- no generic/template-looking sections unless explicitly requested
- no excessive gradients/glows/cards
- no gratuitous animation
- no broken responsive layout
- no inaccessible contrast or focus states
- no missing loading/empty/error states for interactive product UI
- no animation that blocks task completion
- reduced-motion behavior exists where motion is meaningful
- component reuse is sensible
- code is understandable and maintainable

## Motion rules

Motion should have a job. Classify it as:
- **Orientation** — reveals hierarchy or establishes context.
- **Feedback** — confirms an action or state change.
- **Continuity** — connects related states or locations.
- **Emphasis** — directs attention to a meaningful moment.
- **Atmosphere** — optional; use sparingly.

Prefer subtle, composable motion. Avoid stacking parallax + cursor effects + glow + blur + text animation on the same viewport unless the brief explicitly calls for an experimental showcase.

## Resource relevance scoring

When multiple references could apply, score each candidate from 0–3 on:
- semantic fit
- visual fit
- implementation fit
- performance fit
- accessibility fit

Select the smallest set whose combined score is sufficient. Default to 1–3 references per UI problem.

## Output contract

When producing a design/implementation plan, return:
1. **Design direction**
2. **UX structure**
3. **Component/system map**
4. **Selected references and why**
5. **Motion plan**
6. **Implementation plan**
7. **Quality checklist**

When implementing directly, keep the reasoning compact and prioritize working code.

## Important constraints

- Do not reproduce large portions of third-party source code or proprietary prompt libraries.
- Prefer attribution/linking and semantic adaptation when referencing external resources.
- Never select a component only because it looks impressive.
- Never let a component library determine the product's visual identity.
- The design system comes first; components serve the system.
