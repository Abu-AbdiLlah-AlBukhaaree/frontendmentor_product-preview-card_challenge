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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./images/frontend%20mentor%20product%20preview%20card.png)

### Links

- Solution URL: [https://github.com/Abu-AbdiLlah-AlBukhaaree/frontendmentor_product-preview-card_challenge](https://github.com/Abu-AbdiLlah-AlBukhaaree/frontendmentor_product-preview-card_challenge)
- Live Site URL: [https://abu-abdillah-albukhaaree.github.io/frontendmentor_product-preview-card_challenge/](https://abu-abdillah-albukhaaree.github.io/frontendmentor_product-preview-card_challenge/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I gained a lot from the nature of the challenge. The most important thing I learnt is how to use different images for the same position, but with different screen sizes.

This was initially difficult to figure out.

I later thought of setting the `display` of the one I don't need in the screensize I'm working on to `none`

Example:

HTML:

```html
<div class="img-container">
  <img src="./images-1" alt="image 1" class="img-1" />
  <img src="./images-2" alt="image 2" class="img-2" />
</div>
```

CSS:

```css
.img-1 {
  display: block;
}

.img-2 {
  display: none;
}

@media screen and (min-width: 700px) {
  .img-1 {
    display: none;
  }

  .img-2 {
    display: block;
  }
}
```

In the example above, for all screensizes less than 700px, `.img-1` will be visible and `img-2` will be hidden. While for all screensizes greater than 700px, `img-1` will be hidden and `img-2` will be visible.

This functionality can also be achieved using the CSS `visibility` property.

### Continued development

Getting better with building responsive layouts.

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)
