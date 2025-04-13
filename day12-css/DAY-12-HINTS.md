# Day 12 CSS Advanced Techniques

This documentation covers two main topics:
- Day 12-A: Responsive Design with CSS Media Queries
- Day 12-B: CSS Animations and Transitions
- Day 12-C: CSS Transformations

---

# Day 12-A: Responsive Design with CSS Media Queries

This project demonstrates how to create a responsive web page using CSS variables, media queries, and flexbox. Below are key concepts and implementations used:

## CSS Variables

1. CSS variables (Custom Properties) are defined in the `:root` element to maintain consistency throughout the stylesheet:
   ```css
   :root {
     --primary-color: #4361ee;
     --secondary-color: #3a0ca3;
     --mobile-color: #ff595e;
     --tablet-color: #ffca3a;
     --desktop-color: #8ac926;
   }
   ```

2. Variables are accessed using the `var()` function:
   ```css
   .hero {
     background-color: var(--primary-color);
     color: var(--white-color);
   }
   ```

## Media Queries

### Mobile-First Approach
The base CSS targets mobile devices first, then media queries modify the layout for larger screens.

### Types of Media Queries Used

1. **Mobile Portrait Query**:
   ```css
   @media only screen and (max-width: 600px) and (orientation: portrait) {
     /* Styles for mobile phones in portrait orientation */
   }
   ```
   - Targets screens with maximum width of 600px in portrait orientation
   - Uses logical operator `and` to combine multiple conditions

2. **Tablet Query**:
   ```css
   @media screen and (min-width: 601px) and (max-width: 1024px) {
     /* Styles for tablets and medium-sized screens */
   }
   ```
   - Targets screens between 601px and 1024px width
   - Changes layout to two columns in the features section

3. **Negation Query**:
   ```css
   @media not all and (max-width: 400px) {
     /* Styles for screens larger than 400px */
   }
   ```
   - Uses the `not` operator to apply styles to all screens EXCEPT those with width ≤ 400px
   - Adds hover effects to feature boxes on larger screens

4. **Desktop Query**:
   ```css
   @media screen and (min-width: 1025px) {
     /* Styles for desktop screens */
   }
   ```
   - Targets screens larger than 1025px width
   - Changes layout to three columns in the features section

5. **Logical OR Media Query**:
   ```css
   @media screen and (max-width: 480px), screen and (orientation: landscape) and (max-height: 480px) {
     /* Styles for very small screens OR landscape orientation with small height */
   }
   ```
   - Uses comma `,` as logical OR to combine two separate media queries
   - Targets either small screens OR landscape screens with small height

## Responsive Layout Techniques

1. **Flexbox for Layout**:
   - Uses `display: flex` to create responsive layouts
   - Changes `flex-direction` based on screen size:
     ```css
     .feature-container {
       display: flex;
       flex-direction: column; /* Mobile: stacked layout */
     }
     
     @media screen and (min-width: 601px) {
       .feature-container {
         flex-direction: row; /* Tablet/Desktop: side-by-side */
       }
     }
     ```

2. **Visual Indicators**:
   - Color-coded indicators show which screen size is active:
     ```css
     .media-indicator {
       background-color: var(--mobile-color); /* Red for mobile */
     }
     
     @media screen and (min-width: 601px) {
       .media-indicator {
         background-color: var(--tablet-color); /* Yellow for tablet */
       }
     }
     
     @media screen and (min-width: 1025px) {
       .media-indicator {
         background-color: var(--desktop-color); /* Green for desktop */
       }
     }
     ```

3. **Conditional Display**:
   - Uses CSS display property to show/hide content based on screen size:
     ```css
     .mobile-view { display: block; }
     .tablet-view, .desktop-view { display: none; }
     
     @media screen and (min-width: 601px) and (max-width: 1024px) {
       .mobile-view, .desktop-view { display: none; }
       .tablet-view { display: block; }
     }
     ```

## Testing Responsive Design

To test how this page responds to different screen sizes:
1. Open developer tools in your browser (F12 or right-click and select "Inspect")
2. Toggle device toolbar/responsive mode
3. Resize the viewport or select different device presets
4. Observe how the layout, colors, and text indicators change

Try this example code to add a resize event listener that prints the current viewport width:
```javascript
window.addEventListener('resize', function() {
  console.log('Current viewport width: ' + window.innerWidth + 'px');
});
```

---

# Day 12-B: CSS Animations and Transitions

This project demonstrates CSS animation techniques including transitions, keyframe animations, and pseudo-elements. Below are the main concepts implemented with practical examples:

## CSS Transitions

Transitions allow elements to change values over a specified duration, providing smooth effects when properties change.

1. **Basic Transition Syntax**:
   ```css
   .element {
     transition: property duration timing-function delay;
   }
   ```

2. **Hover Transitions with Transform**:
   ```css
   .grow {
     transition: transform 0.3s;
   }
   .grow:hover {
     transform: scale(1.2);
   }
   ```

3. **Multiple Property Transitions**:
   ```css
   .btn {
     transition: all 0.3s;
   }
   ```

## CSS Keyframe Animations

Keyframe animations define animation sequences with multiple steps and can run automatically without user interaction.

1. **Animation Syntax**:
   ```css
   .element {
     animation: name duration timing-function delay iteration-count direction fill-mode;
   }
   ```

2. **Keyframes Definition**:
   ```css
   @keyframes animation-name {
     0% { /* styles at start */ }
     50% { /* styles at middle */ }
     100% { /* styles at end */ }
   }
   ```

3. **Example Animations**:
   - **Fade Animation**: Changes opacity to create fading effect
     ```css
     @keyframes fade-in {
       from { opacity: 0.4; }
       to { opacity: 1; }
     }
     ```
   
   - **Movement Animation**: Uses transform to move elements
     ```css
     @keyframes move-around {
       0% { transform: translateX(0); }
       50% { transform: translateX(30px); }
       100% { transform: translateX(0); }
     }
     ```
   
   - **Bounce Animation**: Combines translateY transforms to create bouncing
     ```css
     @keyframes bounce {
       0%, 100% { transform: translateY(0); }
       50% { transform: translateY(-20px); }
     }
     ```

## CSS Pseudo-classes and Pseudo-elements

1. **Pseudo-classes**: Target special states of elements
   - `:hover`: When user hovers over an element
   - `:first-child`: First element of its type
   - `:last-child`: Last element of its type

2. **Pseudo-elements**: Create and style parts that don't exist in the HTML
   - `::before`: Inserts content before an element's content
   - `::after`: Inserts content after an element's content
   
3. **Interactive Examples**:
   - A tooltip that appears on hover
   - List items that transform on hover
   - Decorative quotes using `::before` and `::after`

## Animation Best Practices

1. **Performance Considerations**:
   - Prefer animating `transform` and `opacity` properties for better performance
   - Use `will-change` property for complex animations

2. **Accessibility**:
   - Provide `prefers-reduced-motion` media query support for users with motion sensitivity
   ```css
   @media (prefers-reduced-motion: reduce) {
     .animated-element {
       animation: none;
       transition: none;
     }
   }
   ```

3. **Testing Animations**:
   - Use browser dev tools to adjust animation speed or pause animations
   - Test across different browsers for consistent behavior

---

# Day 12-C: CSS Transformations

This project demonstrates CSS transform properties that allow you to modify elements' appearance and position without affecting the document flow.

## Basic Transform Functions

1. **Scale**:
   - Changes the size of an element
   ```css
   .scale {
     transform: scale(1.5); /* 1.5 times larger in all directions */
     transform: scaleX(1.5); /* 1.5 times wider */
     transform: scaleY(0.8); /* 0.8 times shorter */
   }
   ```

2. **Rotate**:
   - Rotates an element around a fixed point
   ```css
   .rotate {
     transform: rotate(45deg); /* Rotates 45 degrees clockwise */
     transform: rotate(-90deg); /* Rotates 90 degrees counter-clockwise */
   }
   ```

3. **Translate**:
   - Moves an element from its original position
   ```css
   .translate {
     transform: translateX(30px); /* Moves 30px right */
     transform: translateY(-15px); /* Moves 15px up */
     transform: translate(30px, 15px); /* Moves 30px right, 15px down */
   }
   ```

4. **Skew**:
   - Distorts elements on the 2D plane
   ```css
   .skew {
     transform: skewX(20deg); /* Skews along the X-axis */
     transform: skewY(10deg); /* Skews along the Y-axis */
     transform: skew(20deg, 10deg); /* Skews along both axes */
   }
   ```

## Transform Origin

The `transform-origin` property changes the position of the transformed element's origin:

```css
.box {
  transform-origin: top left; /* Origin at top-left corner */
  transform: rotate(25deg);
}
```

Common values:
- `top`, `right`, `bottom`, `left`, `center`
- Percentage values: `0% 0%` (top-left), `100% 100%` (bottom-right)
- Length values: `20px 30px`

## Combined Transforms

Multiple transform functions can be applied in a single `transform` property:

```css
.combined {
  transform: translateX(20px) rotate(30deg) scale(1.1);
}
```

**Important**: The order matters! Transformations are applied from right to left.

## Using Transforms with Animations

Transforms work well with CSS transitions and keyframe animations:

```css
.box {
  transition: transform 0.3s ease;
}

.box:hover {
  transform: scale(1.5); /* Smooth transition on hover */
}
```

With keyframes:
```css
@keyframes slide {
  0% { transform: translateX(0); }
  25% { transform: translateX(-20%); }
  50% { transform: translateX(-40%); }
  75% { transform: translateX(-60%); }
  100% { transform: translateX(-80%); }
}

.sliding-element {
  animation: slide 8s infinite;
}
```

## Browser Support and Performance

- Transforms are well-supported across modern browsers
- For older browsers, vendor prefixes might be needed:
  ```css
  .box {
    -webkit-transform: scale(1.5);
    -ms-transform: scale(1.5);
    transform: scale(1.5);
  }
  ```
- CSS transforms are hardware accelerated in most browsers, making them performance-friendly
- Prefer transforms over absolute positioning for animations when possible

## Transform vs Positioning

- Transforms don't affect document flow (other elements stay in place)
- Transforms can be animated smoothly with better performance
- Transforms can be applied to inline elements (with `display: inline-block`)
