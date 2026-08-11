# Resource Routing Matrix

This file is the compact routing layer for the five supporting resources.

## Motion Sites

Use when the user asks for:
- landing-page motion direction
- cinematic interaction references
- scroll choreography
- page transitions
- hero animation concepts

Extract: subject + trigger + trajectory + timing + easing + layering + fallback.

## React Bits

Use when the user asks for:
- animated React components
- animated backgrounds
- cursor/magnetic interactions
- text effects
- visual effects that should be implemented as reusable React components

Extract: component category + props/concepts + interaction model + performance constraints.

## Uiverse

Use when the user asks for:
- buttons
- inputs
- toggles
- loaders
- checkboxes
- small UI affordances

Extract the visual/interaction pattern, then normalize it into the project's design tokens. Do not let an isolated element dictate the whole design system.

## Anime.js

Use when:
- CSS transitions are insufficient
- a sequence/timeline needs explicit orchestration
- multiple DOM/SVG properties must be synchronized
- animation needs fine-grained JavaScript control

Prefer CSS or the existing project animation system for simple transitions.

## Aceternity UI

Use when the brief calls for:
- premium landing-page effects
- spotlight/glow interactions
- parallax
- animated cards
- beams/grids
- scroll reveals
- high-impact hero treatments

Use selectively. If an effect becomes the visual identity of the whole page, simplify it and re-author it to match the project's system.

## Cross-resource selection rules

### If the request is mostly static UI

Use shadcn + UI UX Pro Max + Impeccable. Do not force a motion resource.

### If the request is a polished landing page

Use Taste Skill first, then select one motion direction from Motion Sites and at most 1–2 implementation references from React Bits or Aceternity UI.

### If the request is a product dashboard

Prioritize UX, hierarchy, states, density, accessibility, and responsive behavior. Prefer shadcn primitives. Use animation only for feedback and continuity.

### If the request is an experimental showcase

Motion Sites can establish the choreography; React Bits/Aceternity UI can supply implementation patterns; Anime.js can orchestrate custom timelines.

### If the request is a redesign

Audit existing UI first. Preserve useful product behavior, then use Taste Skill + Impeccable to remove visual inconsistency and generic patterns.

## Prompt transformation template

```text
REFERENCE INTENT:
[What problem this reference solves]

TARGET:
[Component / section / page]

VISUAL BEHAVIOR:
[Shape, depth, light, typography, composition]

INTERACTION:
[Trigger and user action]

MOTION:
[Duration, easing, direction, stagger, viewport behavior]

RESPONSIVE:
[Mobile/tablet/desktop changes]

ACCESSIBILITY:
[Keyboard/focus/reduced-motion behavior]

IMPLEMENTATION:
[CSS / React / shadcn / Anime.js / selected reference pattern]

CONSTRAINTS:
[Performance, dependency, browser, project conventions]
```
