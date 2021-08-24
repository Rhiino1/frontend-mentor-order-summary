# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Order summary card solution](#frontend-mentor---order-summary-card-solution)
  - [Table of contents](#table-of-contents)
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

- See hover states for interactive elements
- Have a good summary for their order

### Screenshot

![Desktop](https://i.imgur.com/2D1gdqy.png)
![Mobile](https://i.imgur.com/bM07rMd.png)

### Links

- Solution URL: [Here](https://www.frontendmentor.io/solutions/order-summary-with-html-and-sass-iBfqpbxXE)
- - Live Site URL: [Here](https://rhiino1.github.io/frontend-mentor-order-summary/)

## My process

I Started researching about Semantic HTML5 Markup, it is a very simple but helpful tool i don't often use it. This will help me and anyone that reads this code to easy understand what is on the page. Also, I am going to use SASS, i never use any CSS module and i think this will help me to adapt using more than one .css file and be more "clean" organizing my project. To use SASS I'm going to use GULP tasks, and easy way to add another modules to minify and simplify code.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- [SASS](https://sass-lang.com/) - CSS library

### What I learned

I started this project based on a video series from [Coder Coder](https://www.youtube.com/channel/UCzNf0liwUzMN6_pixbQlMhQ) (Check her channel, She is awesome) just knowing that I am really bad at front end, this is something i want to overpass, i was focusing on back end mostly the time i got interested on web development and leaving front end aside. But when i watched that videos and discovered [Frontend Mentor](www.frontendmentor.io) i just knew this was the tools i need to improve.

One important thing i worked here is responsiveness and breakpoints, i often made my projects responsive and breakpoints made me understand the way to do it, in this case with the SASS help i made something like:
```CSS
// 640px, 1024px, 1400px
$breakpoints-up: ("medium": "40em", "large": "64em", "xlarge": "87.5em");
@mixin breakpoint($size) {
  @media (min-width: map-get($breakpoints-up, $size)) {
    @content;
  }
}
```
(code based from [Coder Coder](https://github.com/thecodercoder/fem-dklt-toggle/blob/main/app/scss/util/breakpoints.scss))

Centering things sometimes just choked for me (Haha frontend memes) so i research a lot just for looking the "best way" to center the card, and finally got this:
```CSS
body {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  ...
}
.container {
  width: 100%;
  min-width: rem(327);
  min-height: rem(567);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: rem(20) 0;
}
```

Also, I use some HTML5 Semantic Markup, thinking this is the best way to make people understand what I'm doing, did some research I that is what I got: 
```html
<main ...>
  <article ...>
    <img ...>
    <h1 ...></h1>
    <p ...></p>
    <section ...>
      <img ...>
      <span ...></span>
      <span ...></span>
      <a ...></a>
    </section>
  </article>
</main>
```

I did my best, but if you have suggestions about that "span", feel free to update it and contact me 😀.

And finally some SASS, i used once a long ago, but it makes me thing that this way to style our html is easy and organized.


### Continued development

Sometimes my grids doesn't work the way I want, so this will be a thing I want to focus on this projects. I want to still working with HTML5 Semantic markup. Using Sass properly and go in depth. In this project I didn't use JavaScript but I have used JavaScript a lot and I guess it's time to use Typescript.

### Useful resources

- [CSS Background](https://devdocs.io/css/background) - This helped me setting the background, I was getting problems but nothing that the documentation could solve.
- [CSS Layout](https://www.w3schools.com/css/css_align.asp) - This is a good examples of Horizontal and Vertical Align.

## Author

- Github - [Cesar SC](https://github.com/Rhiino1)
- Frontend Mentor - [@Rhiino1](https://www.frontendmentor.io/profile/Rhiino1)
- Twitter - [@Rhiino_1](https://www.twitter.com/Rhiino_1)

## Acknowledgments

[Set Up a Real-World Website Project](https://youtu.be/nI0BfXFjI1I) - This video from [Coder Coder](https://www.youtube.com/channel/UCzNf0liwUzMN6_pixbQlMhQ) is an amazing tutorial which helped to understand and set-up my project. I'd recommend it to anyone that want a "project template".