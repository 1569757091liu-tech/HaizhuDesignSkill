# Design Decision Engine

Convert classified intent into a small set of explicit design decisions.

## Decision order

1. Product goal
2. Information hierarchy
3. Layout composition
4. Typography
5. Color
6. Surface/elevation
7. Components
8. Interaction
9. Motion
10. Responsive behavior

## Decision format

```yaml
principle: "short statement"
rationale: "why it serves the user"
constraints:
  - "what must not happen"
implementation_hint: "how the code should express it"
```

## Guardrails

- Every decorative decision needs a reason.
- A visual effect cannot compensate for weak hierarchy.
- Component selection happens after the design language is established.
- Motion is subordinate to task completion.
- Prefer fewer stronger decisions over many weak stylistic details.
