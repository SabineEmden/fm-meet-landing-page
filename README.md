# Frontend Mentor - Meet landing page solution

This is a solution to the [Meet landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/meet-landing-page-rbTDS6OUR). Frontend Mentor challenges help me improve my coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

The brief for this challenge is to build out this landing page and get it looking as close to the design as possible, starting with the following assets:

- Figma design file access
- Mobile, tablet & desktop layouts
- Professional design system for colors, fonts, etc.
- Optimized image assets
- HTML file with pre-written content

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

_Screenshot coming soon_

<!-- ![](./screenshot.jpg) -->

### Links

- _Link to Frontend Mentor solution comming soon_
- [Live site](https://sabineemden.github.io/fm-meet-landing-page/)

## My process

I'm completing this challenge as part of the Frontend Mentor learning path [Building responsive layouts](https://www.frontendmentor.io/learning-paths/building-responsive-layouts--z1qCXVqkD). It is the final of four challenges on this learning path and brings together responsive images, fluid typography, and flexible layouts.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

For the image grid in section one of the landing page, I needed a flexible grid with square cells. The original size of all four images is 510 x 484. I solved this issue by using `aspect-ration: 1` on the grid items.

```html
<div class="gallery">
  <div class="gallery__item">
    <img
      src="./assets/desktop/image-woman-in-videocall.jpg"
      alt="woman in video call on a laptop"
      class="gallery__img"
    />
  </div>
  <!-- four more div.gallery__item -->
</div>
```

```css
.gallery__item {
  aspect-ratio: 1;
  border-radius: var(--spacing-50);
  overflow: hidden;
}

.gallery__img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

### Continued development

Building layouts that are flexible and work well across all screen sizes is a fundamental skill in front-end development. I will be able to us and refine it in future web development projects.

### Useful resources

- [Fluid Typography Tool](https://fluidtypography.com/) - I used this tool to generate the `clamp()` functions for fluid typography.

## Author

I'm an aspiring web developer and a former chemist. What I bring from chemistry to software development is a systematic approach to problem solving and the perseverance to not give up easily.

- Frontend Mentor - [@SabineEmden](https://www.frontendmentor.io/profile/SabineEmden)
- Personal Website - [Sabine Emden](https://www.sabineemden.com/)
- Mastodon - [@sabineemden](https://social.tchncs.de/@sabineemden)

## Acknowledgments

This solution uses a CSS reset based on [A Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/) by Josh Comeau.

The font family in this project is [Red Hat Display](https://fonts.google.com/specimen/Red+Hat+Display). The fonts are licensed under the [Open Font License](https://openfontlicense.org/open-font-license-official-text/).
