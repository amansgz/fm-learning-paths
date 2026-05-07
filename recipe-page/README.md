# Frontend Mentor - Recipe Page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm) , part of learning path [Getting started on Frontend Mentor](https://www.frontendmentor.io/learning-paths/getting-started-on-frontend-mentor-XJhRWRREZd).

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

The goal was to build the optimal layout for the site depending on their device's screen size that closely matches the provided design.

### Screenshot

![Recipe page desktop screenshot](./screenshots/desktop-screenshot.png)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/responsive-recipe-page-with-css-custom-lists-and-table-b3PkL8p9hG](https://www.frontendmentor.io/solutions/responsive-recipe-page-with-css-custom-lists-and-table-b3PkL8p9hG)

- Live Site URL: [https://amansgz.github.io/fm-learning-paths/recipe-page/index.html](https://amansgz.github.io/fm-learning-paths/recipe-page/index.html)

## My process

### Built with

- Semantic HTML5 markup
- BEM Methodology
- CSS custom properties
- Flexbox
- Mobile-first workflow

### Project Structure

```
recipe-page/
|
|--- README.md
|--- index.html
|--- css/
|    |--- base.css
|    |--- main.css
|    |--- tokens.css
|    |--- layout.css
|    |--- components/
|         |--- recipe.css
|         |--- recipe-list.css
|         |--- recipe-table.css
|         |--- footer.css
|--- assets/
|    |---fonts/
|    |---images/
|--- screenshots/ (mobile, tablet and desktop screens)
```

### What I learned

#### Semantic HTML Structure

The `<section>` groups related content (preparation, ingredients, instructions, nutrition).

The section `<header>` contains introductory content (recipe img, title and description).

```html
<!-- Recipe -->
<section>
  <!-- Recipe Header -->
  <header>
    <!-- img, title, description -->
  </header>

  <!-- Recipe Details -->
  <div>
    <!-- Preparation -->
    <section>
      <!-- title, list -->
    </section>

    <!-- Ingredients -->
    <section>
      <!-- title, list -->
    </section>

    <!-- Instructions -->
    <section>
      <!-- title, list -->
    </section>

    <!-- Nutrition -->
    <section>
      <!-- title, description, table -->
    </section>
  </div>
</section>
```

#### CSS styles

Implemented a design system based on the style guide, featuring:

- **CSS custom properties** for colors, font styles and elements spacing
- **Logical properties** for improved layout flexibility
- **rem units** for consistent and responsive scaling

Created custom bullets and counter list using pseudo-elements(`::before`)

```css
.recipe__list li::before {
  content: "\2022";
  position: absolute;
  inset-inline-start: 0;
  inset-block-start: 0;
  font-size: 1rem;
}

.recipe__list--preparation li::before {
  color: var(--rose-800);
}

.recipe__list--ingredients li::before {
  color: var(--brown-800);
}
```

```css
.recipe__list--instructions li::before {
  content: counter(orderedList) ".";
  position: absolute;
  inset-inline-start: 0;
  inset-block-start: 0;
  font-size: 1rem;
  font-weight: var(--fw-semibold);
  line-height: inherit;
  color: var(--brown-800);
}
```

## Author

- Frontend Mentor - [@amansgz](https://www.frontendmentor.io/profile/amansgz)
- Github - [@amansgz](https://github.com/amansgz)
