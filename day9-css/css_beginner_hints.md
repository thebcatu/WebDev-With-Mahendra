# CSS Beginner's Implementation Guide

Follow these hints to recreate the CSS Day 1 learning page:

1. **Create a flex container** to arrange three sections side by side
   ```css
   div { display: flex; justify-content: space-between; }
   ```

2. **Set equal width for each section** with margins for separation
   ```css
   div { width: 30%; margin: 0 10px; }
   ```

3. **Apply different styling methods** for each section:
   - Section 1: Use inline styles (style="property: value;")
   - Section 2: Use internal CSS (inside <style> tags)
   - Section 3: Use external CSS (in day9.css file)

4. **Add rounded corners and shadows** to create visual separation
   ```css
   div { border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
   ```

5. **Create color sample boxes** with flex display
   ```html
   <div style="display: flex; justify-content: space-between;">
     <div style="background-color: #4285f4; color: white;">Color</div>
   </div>
   ```

6. **Style buttons** with no border, background color, and rounded corners
   ```css
   button { background-color: #4285f4; color: white; border: none; border-radius: 5px; }
   ```

7. **Visualize the box model** with visible padding, border, and margin
   ```css
   .box-model { padding: 10px; border: 3px solid #800080; margin: 10px; }
   ```

8. **Demonstrate text styling** with different fonts, sizes, and weights
   ```css
   .font-family-1 { font-family: Arial, sans-serif; }
   .font-size-1 { font-size: 12px; }
   .font-weight-2 { font-weight: bold; }
   ```

9. **Show text alignment options** with separate containers
   ```css
   .text-left { text-align: left; }
   .text-center { text-align: center; }
   .text-right { text-align: right; }
   ```

10. **Demonstrate border styles** with different types
    ```css
    .border-solid { border: 2px solid blue; }
    .border-dashed { border: 2px dashed red; }
    .border-dotted { border: 2px dotted green; }
    ```

11. **Use consistent color schemes** for each section for visual distinction
    ```css
    #section1 { background-color: #ffe4e1; }
    #section2 { background-color: #f0f8ff; }
    #section3 { background-color: #f5f5dc; }
    ```

12. **Style headings** with colored borders to create visual hierarchy
    ```css
    h2 { border-bottom: 2px solid #ff6347; padding-bottom: 5px; }
    ```

---

<div align="center">
    <p><em>Created by <a href="https://github.com/mahendramahara">github: mahendramahara</a></em></p>
</div>
