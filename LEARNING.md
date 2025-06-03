# CSS Sizing Recommendations

## Root Font Size Setup
- Set root `<html>` font-size to **62.5%**, as (1 rem = 16px * 0.625 = 10px... better calculation)

## Using rem Units
- Use **rem** for font-size of most elements
- Use **rem** for margin, padding, border-radius, max-width, etc.

## Using em Units
Use **em** for elements where sizing should be relative to their own font-size:

### Example:
```css
.icon {
    font-size: 1.2em; /* Scales with the parent text */
    margin-right: 0.5em;
}

button {
    padding: 0.8em 1.5em; /* Padding scales with the button's own font-size */
    font-size: 1.8rem; /* Set font-size using rem for consistency */
}
```

## Viewport Units
- Use **vw** or **vh** for specific layout elements or typography that must scale directly with the viewport, e.g, hero section

## Percentage Units
- Use **%** for widths and heights where you want to fill a percentage of the parent

## When to use 'px'?
- While defining **borders**
- For **media query breakpoints**