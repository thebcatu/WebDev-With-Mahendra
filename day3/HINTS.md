# HTML Invoice Design Hints

## Page Structure
- Use `<section>` tags to organize content into logical groups
- Structure content hierarchically with nested sections (main, top, middle, bottom)
- Use semantic HTML elements for better document structure

## Layout Techniques
- Use `display: flex` with `justify-content: space-around` for horizontal layouts
- Apply `display: grid` with responsive columns using `repeat(auto-fit, minmax())`
- Control spacing with `gap`, `margin`, and `padding` properties
- Set container width with percentage values (`width: 60%`) for responsiveness

## Text Styling
- Apply `font-family` for consistent typography throughout the document
- Use `<span>` elements to style portions of text differently
- Apply `text-transform: uppercase` to convert text to all caps
- Use various colors to emphasize different elements

## Images and Graphics
- Size images explicitly with `height` and `width` properties
- Add `border` and `border-radius` to images for styling
- Include `alt` attributes for accessibility
- Position images with margin and alignment properties

## Lists and Tables
- Remove default list markers with `list-style: none`
- Adjust list spacing with `margin` and `padding`
- Style tables with `border-collapse: collapse` for clean borders
- Use `colspan` and `rowspan` attributes to merge table cells
- Apply targeted styling with attribute selectors like `td[colspan="2"]`

## Advanced Styling
- Create highlights with background colors and different text colors
- Use `border-left` to create visual dividers between sections
- Apply consistent styling to related elements
- Use CSS selectors to target specific elements precisely

## Interactive Elements
- Style links with `text-decoration: none` to remove underlines
- Add visual feedback for interactive elements
- Include hover effects for better user experience
- Use contrasting colors for interactive elements

## CSS Organization
- Group related styles together
- Use meaningful class names that describe purpose
- Create reusable style rules for consistent elements
- Consider organizing styles by section (top, middle, bottom)
