# Component Selection Engine

Map approved design decisions to the smallest useful component set.

## Selection order

1. Native HTML / CSS
2. Existing project primitives
3. shadcn primitives
4. Existing project components
5. Supporting reference patterns
6. New dependency only when justified

## Component decision

For each component record:
- user task
- semantic role
- states
- responsive behavior
- accessibility requirements
- visual variant
- dependency requirement

## Anti-patterns

Reject:
- component-first design
- duplicating an existing primitive
- importing a library for one tiny effect when CSS is sufficient
- visually inconsistent components from unrelated libraries
- components whose animation obscures content or controls
