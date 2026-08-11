# Resource Routing Matrix

Use this matrix as a semantic router, not as a catalog. Select the smallest useful set.

| Problem | First choice | Optional companion | Avoid when |
|---|---|---|---|
| Visual direction | Taste Skill | Design MD Collection | The user already supplied a strict design system |
| UX architecture | UI UX Pro Max | Impeccable | The task is purely decorative |
| Visual polish | Impeccable | Taste Skill | The underlying UX is still undefined |
| Standard controls | shadcn | UI UX Pro Max | A project already has equivalent primitives |
| Hero animation | Motion Sites | Aceternity UI / React Bits | Motion distracts from the CTA |
| Scroll reveal | Motion Sites | React Bits | Content must remain instantly scannable |
| Magnetic cursor | React Bits | Anime.js | Touch-first/mobile-only experience |
| Small UI element | Uiverse | shadcn | The element duplicates an existing project primitive |
| Advanced animated hero | Aceternity UI | React Bits | A restrained brand language is required |
| Complex timeline | Anime.js | React Bits | CSS transitions can solve it |
| Background atmosphere | React Bits | Motion Sites | Performance budget is tight |
| Forms/dialogs/tables | shadcn | UI UX Pro Max | A specialized existing system is already in place |

## Scoring

Score each candidate 0–3:

- Semantic fit: does it solve the actual UX problem?
- Visual fit: does it match the established art direction?
- Implementation fit: does it fit the current stack?
- Performance fit: is its runtime cost justified?
- Accessibility fit: can keyboard, reduced-motion, contrast, and touch behavior remain correct?

A candidate should normally score at least 10/15. If several candidates qualify, prefer the one with fewer dependencies and less visual complexity.

## Routing rules

- Never select a resource solely because it is visually impressive.
- Never stack multiple animated libraries for one interaction unless there is a concrete technical reason.
- Prefer shadcn/project primitives for ordinary controls.
- Prefer CSS transitions for simple state changes.
- Prefer React Bits for reusable React-native animated patterns.
- Prefer Anime.js only when choreography/timeline control materially improves the result.
- Prefer Aceternity UI for high-impact showcase patterns, then simplify to fit the product.
- Treat Motion Sites as inspiration/prompt vocabulary rather than source code.
