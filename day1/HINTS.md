# HTML Resume Hints

## Heading Structure
- Use `<h1>` for the main title (Resume)
- Use `<h2>` for section headers (About me, Personal data, Skills)
- Use `<h3>` for subsection headers (Hobbies)

## HTML Structure
- Use `<h1>`, `<h2>`, and `<h3>` for headings to structure content
- Use `<strong>` to emphasize important text
- Utilize `<ul>` (unordered list) and `<ol>` (ordered list) for listing items
- Use `<hr>` to create horizontal dividers for sections

## CSS Styling
- Apply `max-width`, `padding`, `border`, and `margin` properties to style the body
- Example: 
  ```css
  body {
      max-width: 800px;
      padding: 50px;
      border: 5px solid black;
      margin: auto;
  }
  ```

## CSS Styling Tips
- Apply CSS properties like `margin`, `padding`, and `border` to style elements
- Apply the `text-align` property to center align headings
- **Avoid typos** in class names (e.g., `.marign-left` should be `.margin-left`)
- Keep CSS class names meaningful and consistent for better readability

## Text Emphasis
- Use the `<strong>` tag to emphasize important information like field labels
- Example: `<strong>Name</strong>`, `<strong>Email</strong>`, etc.

## Lists
- Use unordered lists (`<ul>`) for skills that don't have a specific order
- Use ordered lists (`<ol>`) for hobbies or steps that have a specific sequence
- Example:
  ```html
  <ul>
      <li>Skill item</li>
  </ul>

  <ol>
      <li>First hobby</li>
  </ol>
  ```

## Text Alignment
- Use the `text-align` CSS property to center align headings
- Example: 
  ```css
  h1 {
      text-align: center;
  }
  ```

## Section Dividers
- Use `<hr>` tags to create horizontal dividers between sections of your resume

## Class Naming
- **Fix the typo**: Change `.marign-left` to `.margin-left` in both CSS and HTML
- Keep class names descriptive and consistent throughout your document
- Example of good class naming: `.personal-info`, `.contact-details`, `.skills-section`

## Section Title
- Use bullet points with hyphens for list items
- When mentioning HTML tags, enclose them in backticks like `<tag>`
- When mentioning CSS properties, use backticks like `property-name`

## Code Examples
- Provide examples in code blocks with the language specified:
  ```css
  selector {
      property: value;
  ```
  
  ```html
  <element attribute="value">content</element>
  ```

## Emphasis
- Use **bold text** for important points or warnings
- Use inline code formatting for `class names`, `element names`, and other code references

## Suggestions
- Provide clear, actionable suggestions
- Reference specific parts of the user's code when applicable
- Use descriptive examples that relate to their project
