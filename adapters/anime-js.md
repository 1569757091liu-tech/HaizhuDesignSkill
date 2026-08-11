# Anime.js Adapter

## Role
Handle animation cases requiring precise timelines or fine-grained JavaScript control.

## Consider when
- multiple elements must coordinate on a timeline
- staggered sequences are central to the experience
- CSS transitions or lightweight React state are insufficient

## Prefer
CSS transitions, Web Animations API, or lightweight React/CSS approaches when they solve the problem cleanly.

## Extract
- timeline
- targets
- trigger
- duration
- easing
- cancellation behavior
- reduced-motion fallback

## Output
An animation specification with an explicit implementation justification.