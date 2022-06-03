# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
### Links

- Solution URL: [Solution Url](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK/hub/four-card-feature-section-wzBhzXh2gW)
- Live Site URL: [Live Url](https://puppychan.github.io/FourCardFeatureSection-FrontendMentor/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- SASS - SCSS

### What I learned

I learn how to use Grid and how to make all cards have the same size with the Grid

Normal Grid:

```css
.proud-of-this-css {
  display: grid;
  grid-template-areas:
  ". b1 ."
  "b2 b1 b3"
  "b2 b4 b3"
  ". b4 .";
}
.box-b1 {
  grid-area: b1;
}
.box-b2 {
  grid-area: b2;
}
.box-b3 {
  grid-area: b3;
}
.box-b4 {
  grid-area: b4;
}
```
However, this code still makes the cards have different height and width. To make them have same size:
```css
.proud-of-this-css {
  display: grid;
  grid-template:
  ". b1 ." 1fr
  "b2 b1 b3" 1fr
  "b2 b4 b3" 1fr
  ". b4 ." 1fr /
  1fr 1fr 1fr;
}
```
The first 4 "1fr" represents the same size in the rows. The last 3 "1fr" represents same width in the columns.
### Continued development

I think I will make 4 cards spinnable if I have time.

## Author

- Github - [Nhung Tran](https://github.com/Puppychan)
- Frontend Mentor - [@Puppychan](https://www.frontendmentor.io/profile/Puppychan)
- LinkedIn [Nhung Tran](https://www.linkedin.com/in/nhung-tran-528396210/)
