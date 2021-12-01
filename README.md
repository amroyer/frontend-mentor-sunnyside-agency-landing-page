# Frontend Mentor - Sunnyside agency landing page solution

This is a solution to the [Sunnyside agency landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/sunnyside-agency-landing-page-7yVs3B6ef). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Links

- Solution URL: [github.com/amroyer/frontend-mentor-sunnyside-agency-landing-page](https://github.com/amroyer/frontend-mentor-sunnyside-agency-landing-page)
- Live Site URL: [glamping-trip.surge.sh](https://glamping-trip.surge.sh)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

The biggest lesson I learned during this project was that different browsers handle images quite a bit differently, especially as grid elements. My first iteration of the image gallery had an issue on Safari where the images were greatly stretched out in the vertical direction. In the end, I think this was because my [CSS reset](https://elad.medium.com/the-new-css-reset-53f41f13282e) has a `max-width: 100%;` property on the images without a corresponding height property. This was ultimately handled with the following CSS on my responsive image elements:

```css
picture img {
  object-fit: contain;
  width: 100%;
}
```

### Continued development

In its current form, the site looks a little strange on tablets, something I should take the time to fix. In addition, it doesn't play well with dark mode at the moment, and at the very least I should take the time to make it look consistent.

## Author

- Frontend Mentor - [@amroyer](https://www.frontendmentor.io/profile/amroyer)
- Twitter - [@amroyerdev](https://www.twitter.com/amroyerdev)
