# Prompt Templates

These templates convert reference-library knowledge into actionable design instructions without dumping entire catalogs into context.

## Design brief

```text
Design a [page/product type] for [target user].
Primary task: [task].
Visual thesis: [one sentence].
Tone: [3–5 adjectives].
Typography: [roles and constraints].
Color: [strategy].
Layout: [grid/container/spacing rhythm].
Surfaces: [flat/border/elevation strategy].
Interaction: [key behaviors].
Motion: [purpose, not decoration].
Responsive: [mobile/tablet/desktop rules].
Accessibility: [focus/contrast/reduced-motion requirements].
Anti-patterns: [what must not appear].
``` 

## Reference extraction

```text
Reference: [resource name]
Problem: [specific UI problem]
Intent: [what the interaction should communicate]
Visual behavior: [shape/light/movement/transition]
Trigger: [hover/click/scroll/load/state]
Timing: [duration/easing/stagger]
Responsive rule: [touch/mobile behavior]
Accessibility fallback: [reduced motion/focus/keyboard]
Implementation preference: [CSS / React / Anime.js / shadcn]
Do not copy source code; adapt the semantic pattern to the current design system.
```

## Component implementation

```text
Build [component] in React + TypeScript.
Use existing project primitives before adding dependencies.
Preserve the established tokens for type, color, radius, spacing, and elevation.
Required states: default, hover, focus-visible, active, disabled, loading, error, success.
Responsive behavior: [rules].
Motion: [purpose + reduced-motion fallback].
Accessibility: semantic HTML, keyboard support, visible focus, adequate contrast.
Keep the implementation composable and avoid one-off magic values where tokens are appropriate.
```

## Review prompt

```text
Audit this UI as a design engineer.
Check hierarchy, spacing, typography, contrast, density, alignment, responsive behavior,
interaction states, accessibility, motion purpose, performance, and component consistency.
Identify the highest-impact problems first.
For each issue provide: problem → why it matters → concrete fix → priority.
Do not recommend decorative changes that do not improve user understanding or task completion.
```
