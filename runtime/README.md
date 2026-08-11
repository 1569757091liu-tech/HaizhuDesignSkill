# Haizhu Design Runtime

The runtime turns a natural-language frontend brief into a structured design decision package before implementation.

## Runtime stages

```text
brief
→ intent classification
→ design decisions
→ resource scoring
→ semantic prompt compilation
→ component mapping
→ motion decision
→ responsive decision
→ implementation plan
→ QA
```

The runtime is deliberately model/tool agnostic. Adapters provide expertise; the runtime decides when expertise is relevant.

## Design principle

Do not optimize for the number of tools called. Optimize for the quality of the final interface.
