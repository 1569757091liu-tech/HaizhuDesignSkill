# Frontend Design QA Checklist

## Visual

- [ ] One clear visual thesis
- [ ] Strong hierarchy at a glance
- [ ] Typography has deliberate roles
- [ ] Spacing follows a repeatable rhythm
- [ ] Color is purposeful rather than decorative
- [ ] Borders, shadows, blur, and gradients are used consistently
- [ ] No accidental template/AI-slop appearance

## UX

- [ ] Primary action is obvious
- [ ] Navigation and information architecture are understandable
- [ ] Loading, empty, error, disabled, success, and retry states exist where relevant
- [ ] Destructive actions have appropriate confirmation
- [ ] Feedback is immediate and understandable

## Responsive

- [ ] Mobile layout is intentionally designed, not merely stacked
- [ ] Touch targets are usable
- [ ] Text remains readable without awkward wrapping
- [ ] Navigation has a mobile strategy
- [ ] Tables/cards do not overflow unexpectedly

## Accessibility

- [ ] Semantic HTML is used
- [ ] Keyboard navigation works
- [ ] `:focus-visible` is visible
- [ ] Contrast is adequate
- [ ] Form controls have labels and useful error messages
- [ ] Motion has a `prefers-reduced-motion` fallback
- [ ] Information is not conveyed by color or motion alone

## Engineering

- [ ] Existing project primitives are reused
- [ ] Tokens/CSS variables are used where practical
- [ ] No unnecessary animation library was introduced
- [ ] Components are composable
- [ ] Dependencies are justified
- [ ] Client-side animation is not used when CSS is sufficient
- [ ] No large third-party source/prompt content was copied

## Motion

- [ ] Every non-trivial animation has a purpose
- [ ] Duration/easing feels consistent
- [ ] Animation does not block task completion
- [ ] Scroll and cursor effects do not overwhelm content
- [ ] Mobile/touch behavior is explicitly considered
