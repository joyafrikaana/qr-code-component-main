# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). 

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



## Overview
his is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H).

### Screenshot

![](screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://qr-code-component-main-ten-dun.vercel.app/)

## My process

For the html, I started off with a section that housed a div witha  class, outerbox. This div housed another div witha class, innerbox. The div innerbox contains the qr code image and another div called box which contaoins the h1 and p element. Initially, the div, bos, didnt exist. The div, innerbox, contained both the qr-code image and the h1 and p element. But, this caused an issue with the styling. While styling the div, innerbox, it automatically took up the width of the h1 and p element which was wider than the the qr-code image. I wanted the div, innerbox to take up the width of the qr-code image and to this, I had to place the h1 and p element in a div called box. This div had a fixed width that was slightly smaller than that of the qr-code image. 

For the CSS, I started with a basic reset, then went ahead witha general body style using the font-family, outfit. Afterwards, I started styling using an im,aginary box model. The display:flex; property, was the backbone of my whole design process, I used this property for my styling and i started the styling from the outermost box and worked my way inward. Only, the qr-code image had a fixed width, every other component had no width. Adding a width led to the project not being centered. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I learned a lot about flex and the correct way to use flex. I also had a bit of practice with media query. Media queries operate in order. Initially, I placed the media query for mobile before that of the tablet, and this definitely made the mobile version wonky. I had to do it the right way, which is placing the media query for the tablet before the mobile. 

```css
.innerbox {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
    background-color: white;
    border-radius: 15px;
    box-shadow: 1px 1px 5px hsl(218, 44%, 22%);
}
.outerbox {
    display: flex;
    justify-content: center;
    background-color: hsl(212, 45%, 89%);
    padding: 50px 300px 50px 300px;
    border-radius: 20px;
    box-shadow: 1px 5px 12px hsl(216, 15%, 48%);
}
```

### Continued development

I'd love to learn more about positioning and why it didn't work with my style. I'd also like to learn more about the relationship between flex and fixed width. The design:flex; didn't work with fixed with nor min or max-width. 

### Useful resources

- [Resource 1](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Media_queries) - This helped me with media query. I really liked this pattern as it was pretty straight forward.
- [Resource 2](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow) - This is an amazing article which helped me finally understand box-shadow. I'd recommend it to anyone still learning this concept.

## Author

- Website - [Joy](https://www.your-site.com)
- Frontend Mentor - [@joafrikaana](https://www.frontendmentor.io/profile/yourusername)

