# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](/images/screenshot.jpg.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Gulp.js] (https://gulpjs.com/)
- [Styled Components](https://styled-components.com/) - For styles

### What I learned

I used CSS Grid on Body element for setting up div element in the center of the viewport: Also used CSS grid to setup elements inside a div element:
And used display: flex to setup price and time elements:

```scss 
body {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
}

.cards {
    align-self: center;
    grid-area: 2 / 2;
}

 ```scss 
 .card {
    display: grid;
    grid-template-areas: 
    "img img img img img img"
    "h2 h2 h2 h2 h2 h2"
    "p p p p p p"
    "pri pri pri time time time"
    "cre cre cre cre cre cre";
    column-gap: rem(60);
    row-gap: rem(10);
 }

```scss
 &__price {
      display: flex;
      align-items: center;
      flex-direction: row;
      flex-wrap: nowrap;
 }
  &__time {
      display: flex;
      align-items: center;
      flex-direction: row;
      flex-wrap: nowrap;
  }



### Continued development

I'm gonna focus working on CSS Grid because I'm not 100% sure how to use it properly.

### Useful resources

- [Example resource 1](https://www.youtube.com/watch?v=rg7Fvvl3taU) - This helped me for Css Grid. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.youtube.com/watch?v=duH4DLq5yoo&t=311s)


## Author

- Website - [Djordje Rajc]
- Frontend Mentor - [@Blurryface1998](https://www.frontendmentor.io/profile/Blurryface1998)
- Twitter - [@Blurryface_1998](https://twitter.com/Blurryface_1998)

