# Frontend Mentor - Blog Preview Card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS), part of learning path [Getting started on Frontend Mentor](https://www.frontendmentor.io/learning-paths/getting-started-on-frontend-mentor-XJhRWRREZd).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Project Structure](#project-structure)
  - [What I learned](#what-i-learned)
    - [Semantic HTML Structure](#semantic-html-structure)
    - [CSS styles](#css-styles)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![Blog preview card desktop screenshot](./screenshots/desktop-screenshot.png)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/blog-preview-card-sDpAD9byf0](https://www.frontendmentor.io/solutions/blog-preview-card-sDpAD9byf0)

- Live Site URL: [https://amansgz.github.io/fm-learning-paths/blog-preview-card/index.html](https://amansgz.github.io/fm-learning-paths/blog-preview-card/index.html)

## My process

### Built with

- Semantic HTML5 markup
- BEM Methodology
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Figma design

### Project Structure

```
blog-preview-card/
|
|--- .gitignore
|--- README.md
|--- index.html
|--- css/
|    |--- base.css
|    |--- main.css
|    |--- tokens.css
|    |--- layout.css
|    |--- components/
|         |--- author.css
|         |--- card.css
|         |--- attribution.css
|--- assets/
|    |---fonts/
|    |---images/
|--- screenshots/ (mobile, tablet and desktop views)
```

### What I learned

#### Semantic HTML Structure

The component uses a single-component architecture with the `article` element, which represents a self-contained, independent composition.

The card `<header>` contains introductory content (image in this case).

The `<div>` groups related content (post metadata, title, description).

The `<time>` tag represents a specific period in time. It's perfect for dates, times, or both.

The `<footer>` contains author information.

```html
<!-- Card blog -->
<article>
  <!-- Card header -->
  <header>
    <img
      src="./assets/images/illustration-article.svg"
      alt=""
      aria-hidden="true"
    />
  </header>

  <!-- Card content -->
  <div>
    <span> Learning </span>

    <div>
      <span>Published</span>
      <time datetime="2023-12-21"> 21 Dec 2023 </time>
    </div>

    <h1>
      <a href="#"> HTML & CSS foundations </a>
    </h1>

    <p>
      These languages are the backbone of every website, defining structure,
      content, and presentation.
    </p>
  </div>

  <!-- Card footer  -->
  <footer>
    <div>
      <img
        src="./assets/images/image-avatar.webp"
        alt="Avatar of Greg Hooper"
      />
      <p>Greg Hooper</p>
    </div>
  </footer>
</article>
```

#### CSS styles

Implemented a design system based on the Figma design and style guide, featuring:

- **CSS custom properties** for colors, font styles and elements spacing
- **Logical properties** for improved layout flexibility
- **rem units** for consistent and responsive scaling
- **prefers-reduced-motion media query** for accessibility

**Adaptive image cropping**: Using image container `height` and blog image `object-fit: cover` to show different image sections - a cropped portion on mobile vs. the complete image on desktop.

```css
.card__header {
  inline-size: 100%;
  block-size: 12.5rem;
}

.card__img {
  inline-size: 100%;
  block-size: 100%;
  object-fit: cover;
}
```

How to apply **stylish borders** to the card using `border` and `box-shadow`

```css
.card {
  border: 1px solid var(--clr-border);
  box-shadow: 8px 8px 0 0 var(--clr-gray-950);
}
```

## Author

- Frontend Mentor - [@amansgz](https://www.frontendmentor.io/profile/amansgz)
- Github - [@amansgz](https://github.com/amansgz)
