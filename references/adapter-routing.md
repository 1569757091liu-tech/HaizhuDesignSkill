# Adapter Routing Matrix

| Problem | Primary | Optional | Usually avoid |
|---|---|---|---|
| Visual identity | Taste | Impeccable | component libraries first |
| UX flow | UI UX Pro Max | Impeccable | decorative resources first |
| Design specification | Design MD | UI UX Pro Max | random component selection |
| Basic primitives | shadcn | Design MD | custom primitive duplication |
| Hero motion | Motion Sites | Aceternity / React Bits | Anime.js unless timeline is needed |
| Scroll choreography | Motion Sites | React Bits / Anime.js | Uiverse |
| Micro interaction | Uiverse | React Bits | Aceternity unless scale warrants it |
| Animated React component | React Bits | Aceternity | Anime.js unless orchestration is required |
| Timeline animation | Anime.js | React Bits | heavy component libraries |
| Showcase effect | Aceternity | Motion Sites / React Bits | stacking multiple effects |
| Existing UI polish | Impeccable | Taste | adding new libraries first |

## Routing rules

1. Solve the product problem before choosing a reference.
2. Establish design direction before high-impact visual effects.
3. Prefer the smallest number of adapters that can fully solve the task.
4. Never use an adapter merely because the user mentioned its library.
5. If the project already has a component/animation system, prefer it over introducing another dependency.
6. External references must be translated into project-native implementation guidance.
7. Accessibility and reduced motion are hard constraints, not optional polish.
