# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Order summary card solution](#frontend-mentor---order-summary-card-solution)
  - [Table of contents](#table-of-contents)
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

- See hover states for interactive elements

### Screenshot

![](/images/screenshot.png)

### Links

- Solution URL: [Frontend Mentor](https://your-solution-url.com)
- Live Site URL: [GitHub Pages Live Site](https://rrincones.github.io/Order-summary-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

For this project, I learned to design for smaller screens first as I wrote the bulk of my CSS code. Known as mobile-first design, it decreases the number of overrides that occur as a result of responsive CSS. Consequently, I wrote only a relatively small block of CSS as part of an @media at-rule, which applies "part of a style sheet based on the result of one or more media queries." The media queries "allow you to apply CSS styles depending on a device's general type (such as print vs. screen) or other characteristics such as screen resolution or browser viewport width." Within the rulesets of the at-rule, I was able to get practice working with the background-image property. I learned how you can have the image repeat as a pattern and stretch it to fill the space. Also, the image appears in front of the element's background color. 

```css
@media (min-width: 769px) {
  body {
    background-image: url("/images/pattern-background-desktop.svg");
    background-size: 100%;
    background-repeat: no-repeat;
  }
  
  main {
    max-width: 28rem;
  }
  
  article {
    padding: 3rem;
  }
}
```
One new thing I put to use in this project is the child combinator, which selects only the chosen element that is the direct child of the chosen parent element. In the example below, I needed to select all the direct children of the article element in order to give them the same bottom margins. The child combinator is the right angle bracket.  

```css
article > * {
  margin-bottom: 1.25rem;
}
```

### Continued development

In general, I just want to keep expanding my knowledge and skills so I'm able to better tackle new challenges. 

### Useful resources

- [Child combinator](https://developer.mozilla.org/en-US/docs/Web/CSS/Child_combinator) - This helped me quickly become familiar with the child combinator. 
- [CSS tutorial](https://www.youtube.com/watch?v=OXGznpKZ_sA) - Chapter 16 of this CSS tutorial helped me learn more about background images. 

## Author

- Frontend Mentor - [@rrincones](https://www.frontendmentor.io/profile/rrincones)
