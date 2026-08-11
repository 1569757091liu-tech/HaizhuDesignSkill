# Resource Scoring Engine

Score a candidate reference from 0–3 on each dimension.

| Dimension | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| Semantic fit | unrelated | adjacent | useful | directly solves problem |
| Visual fit | conflicts | weak | compatible | strongly aligned |
| Implementation fit | impractical | costly | workable | native/simple |
| Performance fit | harmful | questionable | acceptable | lightweight |
| Accessibility fit | conflicts | needs work | acceptable | naturally compatible |

## Selection

`total = semantic + visual + implementation + performance + accessibility`

Default guidance:
- 0–6: reject
- 7–10: consider only if alternatives are weaker
- 11–13: strong candidate
- 14–15: preferred candidate

Do not select more than three supporting references for one UI problem unless the task explicitly requires research breadth.

## Tie-breakers

1. Existing project compatibility
2. Accessibility
3. Performance
4. Simplicity
5. Visual novelty

Novelty is never the primary criterion.