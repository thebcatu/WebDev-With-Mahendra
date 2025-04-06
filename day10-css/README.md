# CSS Properties Demonstration

A colorful, compact demonstration of essential CSS properties in a modern layout.

## Quick Hints

### Display Properties
- `block`: Takes full width, creates line breaks before and after
- `inline`: Takes only needed width, no line breaks
- `inline-block`: Inline element that accepts width/height

### Position Properties
- `static`: Default flow (not positioned)
- `relative`: Positioned relative to normal position
- `absolute`: Positioned relative to nearest positioned ancestor
- `fixed`: Positioned relative to viewport
- `sticky`: Toggles between relative and fixed based on scroll position

### Float vs Position
- Float: Takes element out of flow, content wraps around it
- Position: More control but doesn't allow text wrapping

### Flexbox Tips
- Parent properties: `display: flex`, `justify-content`, `align-items`
- Child properties: `flex-grow`, `flex-shrink`, `flex-basis`
- Use shorthand `flex: grow shrink basis` for efficiency

### Text Styling
- `text-align`: Controls horizontal alignment
- `line-height`: Controls vertical spacing between lines
- `letter-spacing`/`word-spacing`: Controls spacing between letters/words
- `text-decoration`: Underline, overline, line-through
- `text-transform`: Uppercase, lowercase, capitalize

### Color Usage
- Use CSS variables (`--variable-name`) for consistent colors
- Create gradients with `linear-gradient(direction, color1, color2)`
- Consider color contrast for accessibility

### Layout Design
- Grid for overall page structure
- Flexbox for component-level layouts
- Use responsive units and media queries
