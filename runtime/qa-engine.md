# QA / Anti-Slop Engine

Run after implementation and again after major visual changes.

## Gates

### Visual
- hierarchy is obvious
- typography has intentional roles
- spacing rhythm is consistent
- visual identity is distinctive without gimmicks
- effects support content

### UX
- primary task is obvious
- states are complete
- interaction feedback is clear
- no unnecessary cognitive load

### Responsive
- no accidental overflow
- hierarchy survives smaller screens
- touch targets remain usable
- hover-only behavior has a non-hover alternative

### Accessibility
- semantic HTML
- keyboard access
- visible focus
- sufficient contrast
- reduced-motion handling
- labels and accessible names

### Performance
- no unnecessary continuous animation
- no heavy dependency for trivial behavior
- media is reasonably handled
- expensive effects are limited to meaningful surfaces

### Anti-slop
Flag combinations such as:
- generic gradient hero + glass cards + excessive glow
- multiple unrelated visual effects competing for attention
- excessive rounded containers
- decorative animation without semantic purpose
- copied component-library aesthetics that conflict with the product

## Severity

- P0: blocks task/accessibility
- P1: materially harms UX or responsiveness
- P2: noticeable polish issue
- P3: optional refinement

Fix P0/P1 before shipping.