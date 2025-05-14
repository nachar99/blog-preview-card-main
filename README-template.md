# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](.\assets\images\FireShot Capture 003 - Frontend Mentor - Blog preview card* - [blog-preview-card-main-steel-three.vercel.app].png)
![](.\assets\images\FireShot Capture 004 - Frontend Mentor - Blog preview card* - [blog-preview-card-main-steel-three.vercel.app].png)

the two pics are in the assets/images file.

### Links

- Solution URL: [Add solution URL here](https://github.com/nachar99/blog-preview-card-main)
- Live Site URL: [Add live site URL here](https://blog-preview-card-main-steel-three.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom fonts (`@font-face`)
- Flexbox layout
- Box shadow and borders
- Mobile-first responsive design
- CSS pseudo-classes (`:hover`, `:active`)

### What I learned

- **Custom fonts with `@font-face`:** I embedded the Figtree variable font in both regular and italic styles to ensure consistent typography across browsers.

  ````css
  @font-face {
    font-family: 'Figtree';
    src: url('assets/fonts/Figtree-VariableFont_wght.ttf');
    font-style: normal;
    font-weight: 500 800;
  }
  @font-face {
    font-family: 'Figtree';
    src: url('assets/fonts/Figtree-Italic-VariableFont_wght.ttf');
    font-style: italic;
    font-weight: 500 800;
  }

  - **Absolute centering with transform:** I centered the card on the page by combining `position: absolute; left: 50%; top: 50%` with `transform: translate(-50%, -50%)`.

  ```css
  .box {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
  }

  - **Flexbox column layout:** I used Flexbox on the card container to stack content vertically and control spacing naturally.

  ```css
  .box {
    display: flex;
    flex-direction: column;
    padding: 24px;
    gap: 12px;
  }

  ````

- **Interactive states:** I added `:hover` and `:active` pseudo-classes on the article title to give users clear visual feedback when interacting with the text.

  ```css
  h1:hover {
    color: hsl(47, 88%, 63%);
  }
  h1:active {
    color: hsl(47, 88%, 63%);
  }
  ```

### Continued development

Add keyboard focus styles and ARIA attributes for better accessibility.

Explore CSS Grid for more complex, two-dimensional layouts.

Implement a dark mode toggle to switch between light and dark themes.

## Author

- Website - [Abdulrahman Al-Nachar](https://github.com/nachar99)
- Frontend Mentor - [@nachar99](https://www.frontendmentor.io/profile/nachar99)
