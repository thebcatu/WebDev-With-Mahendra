# WebDev-With-Mahendra

## 🧭 Quick Navigator

[View Project Directory Navigator](./index.html)

## Project Navigation

Navigate to different project directories:

- [Day 1 Coding](./day1/)
- [Day 2 Coding](./day2/)
- [Day 3 Coding](./day3/)
- [Day 4 Coding](./day4/)
- [Day 5 Coding](./day5/)

## About This Repository

This repository contains web development projects and exercises created during training sessions with Mahendra.

## Project Structure

The repository is organized by days/topics, with each directory containing specific exercises and projects.

## Getting Started

1. Clone this repository
2. Navigate to any project directory
3. Open the index.html file in your browser or use a local server

## Technologies Used

- HTML5
- CSS3
- JavaScript
- And more as the course progresses

## License

[Add your license information here]

# 📚 Complete HTML Tags Reference Guide

## 📑 Table of Contents
- [Text Formatting](#text-formatting)
- [Document Structure](#document-structure)
- [Content Organization](#content-organization)
- [Forms & Input](#forms-and-input)
- [Media Elements](#media-elements)
- [Tables](#tables)
- [Advanced Features](#advanced-features)
- [SEO & Metadata](#seo-and-metadata)

## Text Formatting
### Basic Formatting
| Tag | Purpose | Example |
|-----|---------|---------|
| `<b>` | Bold text | <b>Bold</b> |
| `<strong>` | Important text | <strong>Important</strong> |
| `<i>` | Italic text | <i>Italic</i> |
| `<em>` | Emphasized text | <em>Emphasized</em> |
| `<mark>` | Highlighted text | <mark>Marked</mark> |
| `<u>` | Underlined text | <u>Underlined</u> |
| `<s>` | Strikethrough | <s>Strikethrough</s> |

### Advanced Text Elements
| Tag | Purpose | Example |
|-----|---------|---------|
| `<abbr>` | Abbreviation | <abbr title="World Wide Web">WWW</abbr> |
| `<cite>` | Work title | <cite>Book Title</cite> |
| `<dfn>` | Definition term | <dfn>HTML</dfn> |
| `<bdo>` | Text direction | <bdo dir="rtl">Reversed</bdo> |
| `<ruby>` | Ruby annotations | <ruby>漢<rt>han</rt></ruby> |

## Document Structure
### Essential Structure
```html
<!DOCTYPE html>
<html lang="en">
    <head>
    </head>
    <body>
        <header>
            <nav></nav>
        </header>
        <main></main>
        <footer></footer>
    </body>
</html>
```

### Semantic Layout
| Tag | Purpose |
|-----|---------|
| `<article>` | Independent content |
| `<section>` | Thematic grouping |
| `<aside>` | Sidebar content |
| `<nav>` | Navigation links |
| `<header>` | Introductory content |
| `<footer>` | Footer information |
| `<main>` | Main content |

## Forms and Input
### Modern Input Types
```html
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file" accept="image/*">
<input type="month">
<input type="number" min="0" max="100">
<input type="range">
<input type="search">
<input type="tel" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
<input type="time">
<input type="url">
```

### Form Validation Attributes
| Attribute | Purpose |
|-----------|---------|
| `required` | Mandatory field |
| `pattern` | Regex pattern |
| `minlength` | Minimum length |
| `maxlength` | Maximum length |
| `min` | Minimum value |
| `max` | Maximum value |

## Media Elements
### Responsive Images
```html
<picture>
    <source srcset="large.webp" media="(min-width: 800px)">
    <source srcset="medium.webp" media="(min-width: 400px)">
    <img src="small.jpg" alt="Responsive image">
</picture>

<figure>
    <img src="image.jpg" alt="Description">
    <figcaption>Image caption</figcaption>
</figure>
```

### Advanced Media
```html
<video controls crossorigin="anonymous">
    <source src="video.mp4" type="video/mp4">
    <track kind="subtitles" src="captions.vtt">
</video>

<audio controls>
    <source src="audio.ogg" type="audio/ogg">
    <source src="audio.mp3" type="audio/mpeg">
</audio>
```

## Interactive Elements
### Modern Components
```html
<details>
    <summary>Click to expand</summary>
    Hidden content
</details>

<dialog>
    Modal content
</dialog>

<progress value="70" max="100">70%</progress>
<meter value="0.6">60%</meter>
```

## SEO and Metadata
```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Page description">
    <meta name="robots" content="index, follow">
    <link rel="canonical" href="https://example.com">
    <meta property="og:title" content="Title">
    <meta property="og:description" content="Description">
    <meta property="og:image" content="image.jpg">
</head>
```

## Security Features
```html
<iframe sandbox="allow-same-origin allow-scripts">
<meta http-equiv="Content-Security-Policy" content="default-src 'self'">
<link rel="manifest" href="/manifest.json">
```

## Accessibility Features
| Tag/Attribute | Purpose |
|---------------|---------|
| `aria-label` | Screen reader label |
| `role` | Element role |
| `tabindex` | Navigation order |
| `alt` | Image description |
| `lang` | Language declaration |

---
> 💡 **Pro Tips:**
> - Use semantic HTML for better SEO and accessibility
> - Validate your HTML using W3C validator
> - Test across different browsers
> - Keep accessibility in mind

---
📅 Last Updated: 2024