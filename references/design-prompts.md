# Design Prompt Patterns

These are reusable semantic prompt patterns. They are intentionally written as original abstractions rather than copied library prompts.

## 1. Distinctive landing page

```text
Create a distinctive, production-ready landing page for [product].
Establish one clear visual concept before choosing components.
Use a strong typographic hierarchy, intentional whitespace, a restrained surface system, and one memorable interaction motif.
Avoid generic SaaS gradients, excessive glassmorphism, repetitive rounded cards, and decorative motion without purpose.
Define desktop/tablet/mobile behavior before implementation.
```

## 2. Premium hero

```text
Design a hero with a single dominant focal point.
Use [visual motif] as the primary depth cue.
Motion should establish hierarchy rather than distract: [entrance / pointer / scroll] with subtle timing and a reduced-motion fallback.
Keep headline readability and CTA clarity above visual effects.
```

## 3. Scroll storytelling

```text
Create a scroll sequence with three stages: establish → reveal → resolve.
Each stage should change one meaningful visual variable at a time.
Use sticky/pinned composition only when it improves comprehension.
Keep scroll progress continuous and avoid abrupt jumps.
Disable or simplify the sequence for prefers-reduced-motion.
```

## 4. Product dashboard

```text
Design a high-density product dashboard around the primary user task.
Prioritize information hierarchy, scanability, keyboard accessibility, responsive behavior, and complete states.
Use shadcn-style primitives for controls and compose them into consistent patterns.
Motion is limited to feedback and continuity.
```

## 5. Component polish

```text
Audit [component] for hierarchy, spacing, typography, contrast, states, focus behavior, responsive behavior, and motion.
Preserve its semantic purpose while removing visual noise.
Return a concise list of high-impact changes, then implement them using the project's existing design tokens.
```

## 6. Motion enhancement

```text
Enhance [component] with one purposeful interaction.
Define trigger, target properties, duration, easing, interruption behavior, and reduced-motion behavior.
Prefer the lightest implementation that achieves the intended effect.
Do not combine multiple attention-grabbing effects unless the composition explicitly requires it.
```

## 7. Reference extraction

```text
Analyze the selected reference only for the current UI problem.
Extract its semantic pattern, not its entire implementation.
Translate it into the project's typography, color, spacing, component architecture, accessibility rules, and responsive behavior.
Return the adapted implementation direction and explain why it fits.
```
