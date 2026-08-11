# shadcn Adapter

## Role
Translate approved design decisions into accessible, project-owned implementation primitives.

## Consider when
- forms, dialogs, menus, tabs, tables, inputs, buttons, sheets, command interfaces, or similar primitives are needed
- the project already uses shadcn/ui

## Rules
- prefer composition over one-off markup
- preserve keyboard and focus behavior
- use project tokens and CSS variables where practical
- do not let component defaults dictate the visual identity
- avoid adding dependencies when a native/project primitive is enough

## Output
Component mapping, composition guidance, state coverage, and implementation notes.