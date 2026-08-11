# Evaluation Rubric

Use this rubric after implementation and again after each repair pass. Score each dimension from 0–3.

| Dimension | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| UX clarity | task is unclear/broken | major friction | mostly clear | immediately clear |
| Visual coherence | inconsistent | several conflicts | coherent | distinctive and intentional |
| System quality | ad hoc markup | partial reuse | good composition | tokenized, reusable system |
| Accessibility | blocking issues | several gaps | minor gaps | keyboard, focus, contrast and motion handled |
| Responsive quality | broken | major layout issues | mostly intentional | mobile/tablet/desktop all deliberate |
| Interaction quality | missing/broken states | basic states only | good feedback | clear, purposeful state transitions |
| Motion quality | distracting/broken | decorative or inconsistent | purposeful | purposeful, restrained, reduced-motion safe |
| Performance | excessive cost | questionable dependencies | acceptable | minimal justified runtime cost |

## Acceptance threshold

- No dimension may score 0.
- UX clarity and accessibility must score at least 2.
- Overall average should be at least 2.25 for normal work and 2.75 for showcase work.
- Any blocking defect overrides the numeric score.

## Repair order

1. Broken primary task or navigation
2. Accessibility blockers
3. Responsive/layout defects
4. Visual hierarchy and content clarity
5. Component consistency
6. Interaction feedback
7. Motion polish
8. Decorative refinement

## Evidence

For each failed dimension, write a concrete observation and the smallest repair that can raise the score. Do not replace a working design merely to chase a higher aesthetic score.
