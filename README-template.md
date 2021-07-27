# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
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

### Screenshot

- Desktop view: (screenshot/screenshot-desktop-view.PNG)
- Mobile view: (screenshot/screenshot-mobile-view.PNG)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop-first workflow

### What I learned

To have the browser choose an image based on the screen size, we use the picture element. The picture element allows us to list a number
of image sources and the conditions they are used in. The final image tag is a fallback for browsers that don't recognise the picture element.
Since the challenge specified which image to use under which conditions, I found that using the picture element gave you control over which image to display.

```html
<picture>
  <source media="(min-width: 700px)" srcset="images/image-header-desktop.jpg" />
  <source media="(min-width: 320px)" srcset="images/image-header-mobile.jpg" />
  <img src="images/image-header-desktop.jpg" alt="" />
</picture>
```

### Continued development

I had trouble adjusting the font sizes according to the screen sizes and will continue to learn more about fluid typography and the use of clamp() and calc() properties.

### Useful resources

- (https://developer.mozilla.org/en-US/docs/Web/HTML/Element/picture) - This MDN doc gives a detailed explanation of the picture element with examples
- (https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images) - In this link there's an explanation to how and when to use the picture element and the srcset property among others for better responsive images.

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)
