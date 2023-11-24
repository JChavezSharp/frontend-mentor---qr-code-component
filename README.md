# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![Screenshot of QR code component](./screenshot.png)


### Links

- Live Site URL: [Live on my GitHub pages](https://jchavezsharp.github.io/frontend-mentor---qr-code-component/)

## My process

### Built with
- HTML5 and CSS3
- CSS Grid

### What I learned

This exercise was a great way to practice what I have been learning about HTML and CSS over the past few weeks. I measured the dimensions of the elements in the provided design screenshots so I could approximate the original as well as possible, I eyeballed some of the sizes and color picked the background and font colors.

The trickiest part was vertically centering the QR code card component without having the scrollbar appear. I centered the card by applying the grid value to the grid property for the body element, I also applied the center value for the place-items property. This automatically centers elements inside grid cells on both axes. I also had to set the height of both the body and html elements to 100vh, doing gets close to the desired result, except the margin of the body needs to be set to 0 so it does not overflow from the html element and causes a scrollbar to appear. Conclusion: never forget about the box model ✏️.  


```css
:root {font-size: 12px;}
    html, body {height: 100vh;}
    body {
      margin: 0;
      display: grid;
      place-items: center;
      background-color: #D5E1EF;
      color: #26334C;
      font-family: sans-serif;
    }
```

### Useful resources

- [Stack Overflow article - how to center element using table without scrollbars](https://stackoverflow.com/questions/53969739/how-to-center-element-using-tables-without-scrollbars) - This helped me realize that the scrollbar was appearing because there was a margin on my body element and needed to set it to 0 for the QR code component to center without creating a scrollbar.
- [FreeCodeCamp - CSS Vertical Align – How to Center a Div, Text, or an Image  ](https://www.freecodecamp.org/news/css-vertical-align-how-to-center-a-div-text-or-an-image-example-code/) - Nice explanation for how to vertically center divs.


## Author

- Frontend Mentor - [@JChavezSharp](https://www.frontendmentor.io/profile/JChavezSharp)
- X aka Twitter - [@JChavezSharp](https://twitter.com/JChavezSharp)


## Acknowledgments

Thanks to Kevin Powell's YouTube channel for his excellent CSS tutorials and to John Duckett for his book HTML & CSS.


