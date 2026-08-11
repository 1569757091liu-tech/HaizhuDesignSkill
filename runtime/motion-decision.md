# Motion Decision Engine

Motion is selected by purpose, not visual fashion.

## Purpose taxonomy

- orientation
- feedback
- continuity
- emphasis
- atmosphere

## Decision rules

1. If motion is not needed for comprehension, feedback, continuity, or emphasis, default to none/subtle.
2. Prefer CSS for simple state transitions.
3. Prefer lightweight React/browser APIs for local interaction.
4. Consider React Bits or Aceternity for reusable animated component patterns.
5. Consider Anime.js only when timeline/orchestration complexity justifies it.
6. Use Motion Sites as a reference for motion language, not as an implementation dependency.

## Required output

```yaml
purpose: "feedback"
trigger: "successful save"
intensity: "subtle"
behavior: "button briefly transitions to confirmation state"
reduced_motion: "retain state change; remove animated transition"
performance: "no continuous animation"
implementation: "CSS transition"
```
