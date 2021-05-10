# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Screenshot](./design/solution-screenshot.png)

### Links

- Solution URL: [github](https://github.com/WidePeepoHappy/stats-preview-card-component)
- Live Site URL: [github pages](https://widepeepohappy.github.io/stats-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- SASS
- BEM

### What I learned

Learned how to use different images for different screen sizes and how to make an overlay.

```html
<div class="card__image">
  <picture>
    <source
      media="(max-width: 375px)"
      srcset="./images/image-header-mobile.jpg"
    />
    <img
      src="./images/image-header-desktop.jpg"
      alt="People working in an office"
      class="card__image--src"
    />
  </picture>
  <div class="card__image--overlay"></div>
</div>
```

```css
&__image {
  position: relative;

  @media (max-width: 375px) {
    height: 240px;
  }

  &--src {
    height: 100%;
  }

  &--overlay {
    position: absolute;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: hsla(277, 94%, 61%, 0.5);
  }
}
```

### Continued development

Need to learn css/sass more. Kind of stumbling around right now.

### Useful resources

- [MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images) - Helped me with images.

## Author

- Frontend Mentor - [@WidePeepoHappy](https://www.frontendmentor.io/profile/WidePeepoHappy)
