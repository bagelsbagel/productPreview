# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](/screenshot.png)

### Links

- Solution URL: (https://github.com/bagelsbagel/productPreview.git)
- Live Site URL: (https://bagelsbagel.github.io/productPreview/)

## My process

I built a product preview using given image assets and recommended styling. I started out by adding content into a container and adjusting the container size and image. I modified the styling of the text and buttons, and lastly, I added a hover and focus state.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Styled Components](https://styled-components.com/) - For styles

### What I learned

I learned how to add a button into HTML and style it accordingly so that it can be interacted with by the cursor. The button also contains an icon with the text, so I did have to modify how it looks.

```html
  <button type="button">
    <img class="icon" src="images/icon-cart.svg" alt="Shopping Cart Icon">
    <p class="button-text">Add to Cart</p>
  </button>
```

I reinforced my learnings on flexbox layouts. This was trickier than the last exercise since I wanted to place an image to the left side, with content (styled text and buttons) to the right. I played around with margin, padding, and alignment until I got it looking good.

```css
body{
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
}
```

For text, one thing I struggled with was getting the text to wrap, or not wrap, where I wanted them to. I figured this out by using overflow-wrap to break text, and white-space to un-wrap text. Note: One fun thing I learned was to style text with different text decorations. For example, line through and small caps.

```css
p{
  overflow-wrap: break-word;
}

p{
  white-space: nowrap;
}
```

### Continued development

I've been testing on desktop rather than mobile, so I will need to check and adjust the mobile design in the future. I've been struggling with finding a way to test and view the design on mobile, and to do mobile-first responsive design. Any help in this area will be much appreciated since I do not know how to start.

### Useful resources

- [Modern CSS](https://moderncss.dev/complete-guide-to-centering-in-css/#vertically-and-horizontally-xy) - This helped me to understand vertical and horizontal centering layouts with flexbox and grid.
- [Dev.to](https://dev.to/daaahailey/css-basic-8-hover-active-focus-4d78) - This article helped me to add basic properties to my button with CSS.

## Author

- Website - [Eileen Lee](https://eileenlee.me/)

## Acknowledgments

-
