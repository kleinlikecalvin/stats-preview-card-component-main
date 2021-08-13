# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout depending on their device's screen size

### Screenshot

![](./images/Screen Shot 2021-08-13 at 11.28.21 AM.png)

### Links

- Solution URL: [My FrontendMentor Solution](https://www.frontendmentor.io/solutions/stat-preview-card-slMBDEiOd)

## My process

At first, I wanted to attempt to accomplish the whole thing without using bootstrap so I could practice the skills that I never learned because Bootstrap was used as a crutch during my initial coding workshops. But, it became frustrating and apparent that this particular project was actually a great time to use Bootstrap. So I imported that and got to building the grid. Once all of the HTML text was set in place I turned my focus to the CSS. It wasn't difficult to clone the card until I reached the colored image overlay. I have previous experience using z-index but I wasn't seeing anyone else use it in their solution to this project, after a while I decided that it was the best use for my project. Then I addressed the "mobile-friendly" version and called it a day.

### Built with

- Semantic HTML5 markup
- Bootstrap
- Google Fonts
- CSS custom properties
- Flexbox

### What I learned

It's been a while since I've practiced my CSS skills so it was fun to dive back into that. I was able to revisit using z-index to accomplish the violet colored overlay used for the image. It was also nice to become reacquainted with Bootstrap. I have a better understanding of gutters/padding now.

```html
<div class="col image">
  <img
    src="./images/image-header-desktop.jpg"
    alt="Three women coding together in an office setting."
    class="px-0 gx-0"
  />
  <div class="overlay"></div>
</div>
```

```css
.col .image {
  margin: 0;
  padding: 0;
  position: relative;
}
.col img {
  margin: 0;
  padding: 0;
  width: 100%;
  border-radius: 0 6px 6px 0;
  z-index: 1;
  position: relative;
  filter: contrast(100%);
}
.overlay {
  background-color: hsl(277, 97%, 54%);
  width: 606px;
  height: 501px;
  z-index: 2;
  position: absolute;
  margin-top: -501px;
  opacity: 45%;
  border-radius: 0 6px 6px 0;
}
```

### Continued development

As I mentioned, I haven't used Bootstrap or CSS in a while (I've been focusing on Java and JS lately) so I'd like to become better with those. CSS seems so powerful to me and intricate, I feel like I've barely scratched the surface. Especially when I read other peoples CSS, they use so many tags/properties that I've never even heard of.

### Useful resources

- [Bootstrap](https://getbootstrap.com/docs/5.0/layout/gutters/) - This helped me understand gutters in Bootstrap a bit better.
- [w3Schools](https://www.w3schools.com/cssref/css3_pr_mediaquery.asp) - This helped me gain a better grasp on media queries to adjust the screen size and configuration.

## Author

- Website - [Nikki Klein](https://www.kleinlikecalvin.com)
- Frontend Mentor - [@streetlightkids](https://www.frontendmentor.io/profile/streetlightkids

## Acknowledgements

- I'd like to thank Nate Walston for continuously being a great mentor.
