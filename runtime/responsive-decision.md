# Responsive Decision Engine

Responsive behavior is designed from content and task priority, not by blindly shrinking desktop layouts.

## Evaluate

- content priority
- navigation strategy
- column collapse
- typography scaling
- touch target size
- density
- image/media cropping
- interaction replacement
- overflow behavior

## Rules

- Define mobile behavior for every major section.
- Preserve primary actions and content hierarchy.
- Replace interactions when hover is unavailable.
- Avoid horizontal overflow unless it is intentional and usable.
- Do not rely on hover as the only way to expose information.
- Test narrow mobile, typical mobile, tablet, and desktop states.

## Output

For each major section:

```yaml
mobile: "single-column; CTA full-width"
tablet: "two-column"
desktop: "asymmetric grid"
interaction_change: "hover preview becomes tap/focus disclosure"
```