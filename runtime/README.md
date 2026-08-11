# Haizhu Design Runtime

The runtime turns a natural-language frontend brief into a structured design decision package before implementation, then validates the implementation through a repair-oriented QA loop.

## Runtime stages

```text
brief
→ intent + constraints
→ design decisions
→ resource scoring
→ semantic prompt compilation
→ component mapping
→ motion decision
→ responsive decision
→ implementation plan
→ QA rubric
→ defect ranking
→ repair loop
→ acceptance
```

The runtime is deliberately model/tool agnostic. Adapters provide expertise; the runtime decides when expertise is relevant.

## v0.6 operating model

### 1. Decide before routing

Extract the user's actual product goal, constraints, stack, and non-goals before selecting any adapter or resource.

### 2. Route minimally

Use the core five tools for their distinct responsibilities. Add Motion Sites, React Bits, Uiverse, Anime.js, or Aceternity UI only when the classified UI problem requires them.

### 3. Compile references, don't copy catalogs

External inspiration becomes semantic implementation guidance that can be adapted to the current project.

### 4. Validate the result

The QA engine scores UX clarity, visual coherence, system quality, accessibility, responsive quality, interaction quality, motion quality, and performance. Failures become repair tasks rather than vague aesthetic criticism.

### 5. Optimize for the interface

Do not optimize for the number of tools called. Optimize for the quality, clarity, maintainability, accessibility, and performance of the final interface.

## Related runtime modules

- `intent-classifier.md` — classify the request.
- `design-decision-engine.md` — establish the design system.
- `resource-scoring.md` — rank supporting references.
- `prompt-compiler.md` — turn references into project-native prompts.
- `component-selection.md` — map decisions to primitives/components.
- `motion-decision.md` — decide whether motion is justified.
- `responsive-decision.md` — define breakpoint behavior.
- `qa-engine.md` — score, rank, and repair defects.

The acceptance rubric is documented in `../references/evaluation-rubric.md`.
