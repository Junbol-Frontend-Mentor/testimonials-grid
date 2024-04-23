# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](./assets/images/screenshot.jpg)

### Links

- Solution URL: (https://github.com/Junbol-Frontend-Mentor/four-card-feature-section)
- Live Site URL: (https://junbol-frontend-mentor.github.io/four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Working with CSS Grid & MediaQueries

```sacss

//-----COLOR SETTINGS ---------------------------------------

// Defining color variables
$colors: (
  'red': hsl(0, 78%, 62%),
  'turquoise': hsl(180, 62%, 55%),
  'orange': hsl(34, 97%, 64%),
  'blue': hsl(212, 86%, 64%),
  'dark-blue-gray': hsl(234, 12%, 34%),
  'light-blue-gray': hsl(229, 6%, 66%),
  'white': hsl(0, 0%, 100%),
  'black': hsl(0, 0%, 0%),
);

//------TYPOGRAPHY SETTINGS ---------------------------------

//Mixing for Typography
// Typography Mixin
@mixin typography() {
  h1 {
    font-family: 'Poppins', serif;
    font-weight: 700;
    font-size: 1.7rem;
    margin-top: -10px; // This pulls the h1 up towards any element above it
    margin-bottom: 1rem;
    color: color('dark-blue-gray'); // Apply the primary text color for headers
    // background-color: bisque; // Background color for visibility
  }

  h2 {
    font-family: 'Poppins', serif;
    font-weight: 200;
    font-size: 1.55em;

    margin-bottom: 0; // No bottom margin to touch h1
    letter-spacing: 0.05em; // Unified letter spacing
    color: color('light-blue-gray'); // Specific color for h2
    // background-color: aqua;
  }

  //------------ Media Queries for Desktop-----------------------------

// Media Queries for Desktop
@media (min-width: 450px) {
  .gridContainer {
    grid-template-columns: 1fr 1fr 1fr; // Define three columns
    grid-template-rows: auto auto; // Define two rows
    align-items: start; // Align items to the start of their grid area
  }

  .card {
    // Supervisor card takes the first column and spans two rows
    &:nth-child(1) {
      grid-column: 1;
      align-self: center;
      grid-row: span 2; // Spans two rows
    }

    // Team Builder card takes the second column, first row
    &:nth-child(2) {
      grid-column: 2;
      grid-row: 1; // First row of the second column
    }

    // Karma card takes the second column, second row
    &:nth-child(3) {
      grid-column: 2;
      grid-row: 2; // Second row of the second column
    }

    // Calculator card takes the third column and spans two rows
    &:nth-child(4) {
      grid-column: 3;
      align-self: center;
      grid-row: span 2; // Spans two rows
    }
  }
}
```

### Continued development

I would like to continue studying responsive CSS specially with Grid + Flexbox and Css animation, transitions and FX like parallax.

### Useful resources

- [web.dev](https://web.dev/learn/css) - This helped me for get back on track with CSS.
- [w3schools](https://www.w3schools.com/css/default.asp) - The one place to refresh stuff in practical way.

## Author

- Website - [Junier Bolivar](https://www.bolivarcreativedesign.com)
- Frontend Mentor - [Junbol](https://www.frontendmentor.io/profile/Junbol)
- Twitter - [@JunierBolivar](https://www.twitter.com/@JunierBolivar)

## Acknowledgments
