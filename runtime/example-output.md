# Runtime Example

User brief:

> Build a premium AI SaaS landing page with a memorable hero and tasteful motion.

## Compiled result

```yaml
surface: landing-page
primary_problem:
  - visual-direction
  - motion
  - conversion
visual_intensity: premium
motion_intensity: interactive

core_adapters:
  - Taste
  - UI UX Pro Max
  - Design MD
  - Impeccable
  - shadcn

supporting_candidates:
  Motion Sites: 13/15
  Aceternity UI: 13/15
  React Bits: 11/15
  Anime.js: 8/15
  Uiverse: 5/15

selected:
  - Motion Sites
  - Aceternity UI

motion:
  purpose: orientation
  hero: restrained focal interaction
  reduced_motion: static equivalent

implementation:
  stack: React + TypeScript
  primitives: shadcn where applicable
  animation: CSS/lightweight React first
  new_dependency: only if complexity requires it

anti_patterns:
  - excessive glow
  - glassmorphism everywhere
  - competing hero effects
  - animation that delays the CTA
```

The important behavior is that the runtime does not select every available library. It selects the smallest useful set and explains why.