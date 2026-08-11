# Prompt Compiler

The compiler converts external references into implementation-ready semantic prompts.

## Input

- user intent
- design decisions
- selected adapters
- selected references
- technical stack
- accessibility/performance constraints

## Output schema

```yaml
intent: "what the interaction accomplishes"
target: "element or section"
visual_behavior: "what users see"
interaction_trigger: "what causes it"
motion:
  duration: "approximate range or qualitative value"
  easing: "qualitative easing"
  sequence: "ordered behavior"
responsive: "mobile/tablet/desktop behavior"
accessibility: "keyboard, focus, reduced motion, contrast behavior"
implementation: "preferred project-native technique"
avoid:
  - "anti-pattern"
```

## Rules

- Preserve the design intent, not the source implementation.
- Do not copy large third-party snippets.
- Prefer existing project primitives.
- Replace library-specific nouns with semantic behavior when possible.
- Make animation optional when it is not essential to comprehension or feedback.
