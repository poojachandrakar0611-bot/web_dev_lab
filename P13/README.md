# P13: Choosing Between Flexbox and Grid for a Shared Layout

## Aim
Compare Flexbox and CSS Grid by creating similar card layouts with both layout systems.

## Comparison

| Flexbox | CSS Grid |
|---|---|
| Mainly works in one dimension: a row or a column. | Works in two dimensions: rows and columns. |
| Useful for navigation bars, button groups, and aligning items. | Useful for page sections, galleries, and card layouts. |
| Items can grow, shrink, and wrap along the flex axis. | Tracks can be defined with `fr`, `minmax()`, and repeat patterns. |

## Files
- `index.html` — contains both layout examples.
- `style.css` — uses Flexbox for one list and Grid for the other.

## Procedure
1. Save both files in a folder named `P13`.
2. Open `index.html` in a browser.
3. Compare the Flexbox navigation-style cards with the Grid project cards.
4. Resize the browser to see how both layouts respond.

## My conclusion
I would choose Flexbox when I mainly need to align items in one row or column, such as a navbar. I would choose Grid when I need to control both rows and columns, such as a project gallery. Both can be used together in the same page.
