# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Blog preview card solution](#frontend-mentor---blog-preview-card-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

desctop  
![desktop](./images/screenshot_desktop.png)

mobile  
![mobile](./images/screenshot_mobile.png)

### Links

- Solution URL: [st0272\/fm-blog-preview-card](https://github.com/st0272/fm-blog-preview-card/)
- Live Site URL: [fm-blog-preview-card](https://st0272.github.io/fm-blog-preview-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

Styling card links using pseudo-elements

```css
.card__link {
    ...
    &::after {
        content: "";
        position: absolute;
        inset: 0;
    }
}
```

Hover styles applied only on desktop devices and focus styles applied only on touch screen device

```css
@media (any-hover:hover) and (pointer: fine) {
  .card__link:hover {
      color: var(--yellow);
  }

  .card:hover {
        .card__description {
            color: var(--gray-500);
        }
    }
}

@media (any-hover:none) and (pointer:coarse) {
    .card__link:focus {
        color: var(--yellow);
    }

    .card:focus {
        .card__description {
            color: var(--gray-500);
        }
    }
}
```

## Author

- Website - [Suzunatsu Website](https://www.suzunatsu.com)
- Frontend Mentor - [@st0272](https://www.frontendmentor.io/profile/st0272)
- Twitter - [@suzuantsu_](https://www.twitter.com/suzuantsu_)