# Tool Adapter Architecture

Adapters define the contract between HaizhuDesignSkill and external design resources.

Each adapter answers five questions:

1. When should this resource be considered?
2. What context should be sent to it?
3. What output should be extracted?
4. When should it be rejected?
5. How should its output be translated into implementation guidance?

## Core adapters

- `taste.md` — visual direction and anti-slop judgment
- `impeccable.md` — visual/UX audit and refinement
- `ui-ux-pro-max.md` — UX patterns and design-system reasoning
- `design-md.md` — structured design specification
- `shadcn.md` — implementation primitives

## Supporting resource adapters

- `motion-sites.md`
- `react-bits.md`
- `uiverse.md`
- `anime-js.md`
- `aceternity-ui.md`

## Adapter lifecycle

```text
brief
  ↓
classify problem
  ↓
select adapter(s)
  ↓
extract semantic guidance
  ↓
score candidate references
  ↓
translate into project-native decisions
  ↓
implement
  ↓
audit
```

An adapter is a decision layer, not a proxy for blindly copying an external library.