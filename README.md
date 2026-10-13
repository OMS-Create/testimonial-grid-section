```markdown
# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.[cite: 2]

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-I-learned)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size[cite: 2]

### Screenshot

![Screenshot](./images/Screenshot.png)

### Links

- Solution URL: [solution URL](https://testimonial-grid-section.vercel.app)[cite: 2]
- Live Site URL: [live site URL](https://github.com/OMS-Create/testimonial-grid-section)[cite: 2]

## My process

### Built with

- Semantic HTML5 markup[cite: 2]
- CSS custom properties (variables for theme colors)[cite: 1, 2]
- CSS Grid (using template areas for desktop layout)[cite: 1, 2]
- Flexbox for internal card alignment[cite: 1, 2]
- Mobile-first / Portrait orientation responsive workflow[cite: 1, 2]
- Google Fonts ('Barlow Semi Condensed')[cite: 1]

### What I learned

Working through this project, I strengthened my skills in CSS Grid layout techniques, specifically mapping out complex component areas:

```css
.grid-section {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto auto;
  grid-template-areas: 
  "daniel daniel jonathan kira"
  "jeanette patrick patrick kira";
  gap: 1.875rem;
  max-width: 69.375rem;
}

```

I also implemented orientation-based media queries to handle stacking behavior gracefully on portrait screens:

```css
@media (orientation: portrait) {
  .grid-section {
    grid-template-columns: 1fr;
    grid-template-areas: 
    "daniel"
    "jonathan"
    "jeanette"
    "patrick"
    "kira";
  }
}

```

## Author

- Frontend Mentor - [@OMS-Create](https://www.frontendmentor.io/profile/OMS-Create)

## Acknowledgments

Thanks to [Frontend Mentor](https://www.frontendmentor.io/) for the challenge and the supplied design assets.