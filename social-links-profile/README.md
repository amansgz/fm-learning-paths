# Frontend Mentor - Social Links Profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ) , part of learning path [Getting started on Frontend Mentor](https://www.frontendmentor.io/learning-paths/getting-started-on-frontend-mentor-XJhRWRREZd).

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

![Social links Profile desktop screenshot](./screenshots/desktop-screenshot.png)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/social-links-profile-bb8VPCELhQ](https://www.frontendmentor.io/solutions/social-links-profile-bb8VPCELhQ)

- Live Site URL: [https://amansgz.github.io/fm-learning-paths/social-links-profile/index.html](https://amansgz.github.io/fm-learning-paths/social-links-profile/index.html)

## My process

### Built with

- Semantic HTML5 markup
- BEM Methodology
- CSS custom properties
- Flexbox
- Mobile-first workflow

### Project Structure

```
social-links-profile/
|
|--- README.md
|--- index.html
|--- css/
|    |--- base.css
|    |--- main.css
|    |--- tokens.css
|    |--- layout.css
|    |--- components/
|         |--- profile.css
|         |--- profile-social.css
|         |--- attribution.css
|--- assets/
|    |---fonts/
|    |---images/
|--- screenshots/ (mobile, tablet and desktop screens)
```

### What I learned

#### Semantic HTML Structure

The component uses a single-component architecture with the `article` element, which represents a self-contained, independent composition.

The card `<header>` contains introductory content (profile user in this case).

```html
<article>
  <!-- profile header with profile info (avatar, name, location and bio) -->
  <!-- profile-social -->
</article>
```

#### CSS styles

Implemented a design system based on the style guide, featuring:

- **CSS custom properties** for colors, font styles and elements spacing
- **Logical properties** for improved layout flexibility
- **rem units** for consistent and responsive scaling
- **prefers-reduced-motion media query** for accessibility

## Author

- Frontend Mentor - [@amansgz](https://www.frontendmentor.io/profile/amansgz)
- Github - [@amansgz](https://github.com/amansgz)
