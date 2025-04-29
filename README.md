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

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot_desktop.png)
![](./screenshot_mobile.png)
![](./screenshot_state.png)

### Links

- Solution URL: [https://github.com/skhbabez/blog-preview-card-main](https://github.com/skhbabez/blog-preview-card-main)
- Live Site URL: [https://skhbabez.github.io/blog-preview-card-main/](https://skhbabez.github.io/blog-preview-card-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS
- Flexbox
- Mobile-first workflow

### What I learned

I mostly focused on semantic markup and responsiveness. I took a deep dive into semantic html elements and put a lot of thought into how to lay them out and utilize them for this challenge. For responsiveness i looked at alternatives for using media queries, since the layout is so simple and learned about the clamp function.

```css
.card section h1 {
  font-weight: 800;
  font-size: clamp(2rem, 3.6vw, 2.4rem);
  line-height: 150%;
}
```

Furthermore, I tried to utilize rem more, which made this challenge a lot easier conbining it with dynamic vw values. I especially did not know about that trick to reset the root font to 10 px with a percentage value, to make sure font sizes can still adjusted in the browser dynamically.

```css
html {
  font-size: 62.5%;
}

body {
  background-color: var(--yellow);
  font-size: 1.6rem;
}
```

### Continued development

Next step should be diving deeper into responsive design tools in CSS and practicing more. I am also gonna focus more on comin gup with better layouts incorporating semantic elements. I feel like I can't use them that intuitively yet.

### Useful resources

- [Clamp function](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp) - Really useful tool I did not knew about.
- [rem discussion](https://stackoverflow.com/questions/30374863/why-use-rem-instead-px-when-its-the-same-anyway) - Helped me get a better grasp on how to incorporate rem in projects in a responsive way
