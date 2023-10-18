# Frontend Mentor - Sunnyside agency landing page solution

This is a solution to the [Sunnyside agency landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/sunnyside-agency-landing-page-7yVs3B6ef). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

-   [Overview](#overview)
    -   [The challenge](#the-challenge)
    -   [Screenshot](#screenshot)
    -   [Links](#links)
-   [My process](#my-process)
    -   [Built with](#built-with)
    -   [What I learned](#what-i-learned)
-   [Author](#author)

## Overview

### The challenge

Users should be able to:

-   View the optimal layout for the site depending on their device's screen size
-   See hover states for all interactive elements on the page

### Screenshot

![](./assets/screenshots/siteref3.jpg)

### Links

-   Solution URL: [Solution](https://www.frontendmentor.io/solutions/responsive-landing-page-bootstrap-sass-NEk2PZ8ng4)
-   Live Site URL: [Live site](owaruuu.github.io/sunnyside-landing-page-frontend-mentor-challenge-4/)

### Built with

-   Semantic HTML5 markup
-   CSS custom properties
-   Flexbox
-   Mobile-first workflow
-   [Sass](https://sass-lang.com) - CSS Extension
-   [Bootstrap](https://getbootstrap.com) - Frontend Framework

### What I learned

- How to make the color underline in the 'learn more' links

I wrapped the a link inside a div along with an empty div that I style to give it the look I wanted
```html
<div class="link-group">
    <a href="">Learn more </a>
    <div class="first-link-bar"></div>
</div>
```

Used 'display: content:' to avoid incrementing the area for :hover
```css
.link-group {
    display: content;

    :hover {
        .first-link-bar {
            border-color: $yellow;
        }
    
        .second-link-bar {
            border-color: $soft-red;
        }
    }
}

.first-link-bar,
.second-link-bar {
    width: 130px;
    border-radius: 13px;
    position: relative;
    left: -5px;
    top: -10px;
    z-index: -1;
}
```
The parent div itself receives the :hover but the empty divs inside are what is modified

## Author

-   Linkedin - [Josue Marquez](https://www.linkedin.com/in/josuemarquez/)
-   Frontend Mentor - [@owaruuu](https://www.frontendmentor.io/profile/owaruuu)
