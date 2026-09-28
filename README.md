# Assignment 2 – One HTML, Two Styles

## File organization
- `index.html` – single HTML page with six `div.box` elements (A–F). The `<link>` tag decides the look:
  `styleA.css` (Version A) or `styleB.css` (Version B).
- `styleA.css` – vertical layout: Flexbox column with `justify-content: space-around`, alternating box colors, styled last box.
- `styleB.css` – horizontal layout: Flexbox row with `flex-wrap: nowrap`, dotted left border, hover effect, last box `position: fixed` in the bottom-right corner.

## Challenges
- Getting equal vertical spacing that changes with window size while boxes never overlap or resize:
  solved with `space-around`, `flex: none`, and a minimum body height.
- Keeping boxes on one line in Version B: `flex-wrap: nowrap` plus `flex: none` so they don't shrink.
- Placing the last box in the corner: `position: fixed` takes it out of the flex row.
- Centering the text vertically in the last box of Version A: made that box its own flex container.
