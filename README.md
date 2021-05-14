# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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

Responsive stats preview card

### Links

- [Solution URL](https://www.frontendmentor.io/solutions/css-flexbox-and-grid-wctB-03EO)
- [Live Site URL](https://hk273.github.io/SP-Card/)

## My process


### Built with

- HTML5
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned

- Multiple media queries
- More CSS grid
- Flexbox
- BEM: Block Element Modifier naming convention
- CSS custom variables


```css

/* Custom Properties  */
:root {
    --main-background: hsl(233, 47%, 7%);
    --card-background: hsl(244, 38%, 16%);
    --accent: hsl(277, 64%, 61%);
    /* main heading, stats */
    --white: hsl(0, 0%, 100%);
    /* main paragraph */
    --transparent-white-p: hsla(0, 0%, 100%, 0.6);
    /* stat headings */
    --transparent-white-h: hsla(0, 0%, 100%, 0.75);
    --gray: hsl(0, 0%, 95%);
    --font-Inter: "Inter";
    --font400: "Lexend Deca";
}


```
```css
/* Responsive breakpoints */

@media screen and (max-width: 1000px) {
    .wrapper {
        display: grid;
        /* collapse to rows */
        grid-template-columns: none;
        position: relative;
        width: 70%;
        height: 50%;
        /* Centre content on page*/
        top: 4rem;
    }
    body {
        padding-bottom: 10rem;
    }
    .col-two {
        border-top-left-radius: 1rem;
        border-bottom-left-radius: 0;
        border-bottom-right-radius: 0;
        width: 100%;
        height: 100%;
        /* Reverse grid order */
        grid-row: 1;
    }
    .col-one {
        text-align: center;
        border-top-left-radius: 0;
        border-bottom-right-radius: 1rem;
    }
    .card {
        width: 0;
    }
    img {
        border-bottom-right-radius: 0;
    }
}


/* Allign stat items in rows */

@media screen and (max-width: 600px) {
    .cards {
        display: block;
        flex-direction: row;
        /* Wrap to rows when screen re-sized */
        margin-left: 33%;
        margin-top: -2.5rem;
        line-height: 1.8;
    }
}
```

### Continued development

- Mobile first design
- Flexbox
- Responsive design


### Useful resources

- [Resolving file path](https://stackoverflow.com/questions/7327011/cant-set-background-image-in-css/7327020)
- [Add overlay to image](https://dev.to/ellen_dev/two-ways-to-achieve-an-image-colour-overlay-with-css-eio)
- [Object-fit](https://www.w3schools.com/css/css3_object-fit.asp) 
- [Justify-Content control spacing](https://stackoverflow.com/questions/42080123/controlling-the-amount-of-space-in-justify-content-space-between) 
- [Cards / Stats Section](https://codepen.io/kevinpowell/pen/LYxGNaK?editors=1100) 
- [Reverse grid order at breakpoint](https://stackoverflow.com/questions/45383042/reverse-order-of-columns-in-css-grid-layout)  


## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)

## Acknowledgments

Brilliant resources created by these guys!

- [Kevin Powell](https://www.youtube.com/user/KepowOb)
- [DesignCourse](https://www.youtube.com/channel/UCVyRiMvfUNMA1UPlDPzG5Ow)

