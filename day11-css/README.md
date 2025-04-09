# Day 11 - CSS Layout Tasks

This document provides hints and guidance for completing two different layout tasks - one using CSS Flexbox and another using CSS Grid.

---

## Day11-A: Flexbox Landing Page

This task demonstrates how to create a responsive landing page using **HTML** and **CSS Flexbox**.

### Preview:
![Flexbox Layout](https://i.ibb.co/D9vPjDj/flexbox-preview.jpg)

### HTML Structure:
1. **Two-Column Layout**:
   - Create a header section at the top
   - Use `<div>` elements to create a left column for the form and a right column for the showcase
   - Example tags: `<div>`, `<form>`, `<fieldset>`, `<legend>`, `<input>`, `<textarea>`, `<select>`, `<button>`

2. **Form Elements**:
   - Include fields like text input, email input, dropdowns, radio buttons, checkboxes
   - Add proper labels and a submit button
   - Group related elements using `<fieldset>` and `<legend>`

3. **Showcase Section**:
   - Create cards with headings, paragraphs, buttons, and lists
   - Add visual indicators like tags and badges
   - Organize cards in rows using nested flex containers

### CSS Styling:
1. **Flexbox Layout**:
   - Use `display: flex;` on container with `flex-direction: column` for the page
   - Apply `display: flex;` with `flex: 1` for the main columns
   - Use nested flex containers for card layout 

2. **Styling Techniques**:
   - Apply `box-shadow` for cards and form elements
   - Use `:hover` effects for interactive elements
   - Create custom list styling
   - Add `border-radius` for rounded corners

### Color Palette:
| Color Name       | Hex Code   | Usage                          |
|------------------|------------|--------------------------------|
| Primary Blue     | `#4a90e2`  | Buttons, headers, and accents  |
| Dark Blue        | `#357abd`  | Hover effects and gradients    |
| Light Gray       | `#f5f5f5`  | Background color               |
| White            | `#ffffff`  | Form backgrounds and cards     |
| Highlight Red    | `#e74c3c`  | Tags and alerts                |
| Success Green    | `#28a745`  | Primary action buttons         |
| Neutral Gray     | `#6c757d`  | Secondary buttons and badges   |

---

## Day11-B: CSS Grid Layout

This task demonstrates how to create a dynamic grid-based layout using **HTML** and **CSS Grid** (without Flexbox).

### Preview:
![Grid Layout](https://i.ibb.co/HTXJSsY/grid-preview.jpg)

### HTML Structure:
1. **Grid Container**:
   - Create a main container for the grid layout
   - Include sections for header, images, content areas, and footer
   - Use semantic HTML5 elements where appropriate: `<header>`, `<section>`, `<footer>`

2. **Image Grid**:
   - Add multiple image items with captions
   - Use different sizes/positions for visual interest
   - Include hover effects for images

3. **Content Sections**:
   - Create text sections with headings, paragraphs
   - Add a list section with custom styling
   - Use different text formatting styles

### CSS Grid Implementation:
1. **Grid Layout**:
   - Use `display: grid;` on the main container
   - Define `grid-template-areas` to name and arrange grid sections
   - Set `grid-template-columns` and `grid-template-rows` for layout structure
   - Apply appropriate `gap` between grid items

2. **Responsive Design**:
   - Add media queries for tablet and mobile layouts
   - Adjust grid areas and columns for different screen sizes
   - Maintain visual hierarchy across screen sizes

3. **Visual Styling**:
   - Apply gradient backgrounds for the header
   - Use box-shadow for depth
   - Create custom list styling
   - Add hover effects and transitions

### Color Palette:
| Color Name       | Hex Code   | Usage                          |
|------------------|------------|--------------------------------|
| Orange           | `#ff9966`  | Gradients and accents          |
| Red-Orange       | `#ff5e62`  | Headers, buttons, and text     |
| Yellow           | `#ffdd57`  | Highlights and accents         |
| Light Gray       | `#f0f2f5`  | Background color               |
| White            | `#ffffff`  | Content cards background       |
| Dark Gray        | `#333333`  | Main text color                |

### Image Resources:
For both tasks, you can use these image resources:
- Nature: https://images.pexels.com/photos/2662116/pexels-photo-2662116.jpeg
- Architecture: https://images.pexels.com/photos/323705/pexels-photo-323705.jpeg
- Technology: https://images.pexels.com/photos/3861969/pexels-photo-3861969.jpeg
- Travel: https://images.pexels.com/photos/1271619/pexels-photo-1271619.jpeg

---

## Key Differences Between Tasks:

1. **Day11-A (Flexbox)**:
   - One-dimensional layout system (rows OR columns)
   - Good for content flow and alignment within containers
   - Two-column layout with nested flex containers
   - Blue color scheme

2. **Day11-B (Grid)**:
   - Two-dimensional layout system (rows AND columns)
   - Excellent for overall page layout and complex arrangements
   - Various sized grid areas with named template areas
   - Orange-red color scheme

Complete both tasks to understand the strengths and use cases for each layout system!
