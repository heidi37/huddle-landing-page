# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size (375px and 1440px wide were specified in the design mockups)
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://www.frontendmentor.io/solutions/responsive-accessible-landing-page-using-semantic-html5-and-css3-Xo2uyKAPF)
- Live Site URL: [Add live site URL here](https://heidi37.github.io/huddle-landing-page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow


### What I learned

I had to refresh a little bit about the "fill" on an svg. You need to add the svg code directly to the html if you want access to it in the DOM. So instead of pulling in the svg files for the social media icons with the img tag I placed the svg code directly in the html and then I could access the hover state with css.


```css
.social:hover {
    fill: #e882e8;
    border-color: #e882e8;
}
```

When I html validated my code I had an error because I trued to use the alt attribute on an svg tag. This is not the appropriate way to make svg files accessible. Instead I needed to use aria tags in combination with a title tag.

```html
<svg class="social" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512" aria-labelledby="facebookID">
<!-- Font Awesome Free 5.15.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) -->
<title id="facebookID">Facebook Icon</title>
<path d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z" />
</svg>
```


### Continued development

I could have used flexbox or CSSgrid to build this page but it was such a simple page I chose not to refresh my memory on those today. For future and more complicated layouts I would utilize CSSgrid or flexbox.


### Useful resources

- [CSS Tricks](https://css-tricks.com/accessible-svgs/) - This helped me figure out how to make svgs directly embedded in the html accessible.
- [Stack Overflow](https://stackoverflow.com/questions/19157122/css-change-fill-color-on-hover-svg-path) - This helped me remember how to change the hover state on an svg.



## Author

- Website - [Heidi Fryzell](https://heidifryzell.com)
- Frontend Mentor - [@heidi37](https://www.frontendmentor.io/profile/heidi37)
- Twitter - [@HeidiFryz](https://www.twitter.com/heidifryz)



