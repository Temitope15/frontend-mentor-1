# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Refactoring process](#refactoring-process)
  - [Useful resources](#useful-resources)
- [Author](#author)



## Overview

### Screenshot

![](./images/QR_CODE-SCREENSHOT.png)


### Links

- Solution URL: [GitHub Source Code](https://github.com/Temitope15/frontend-mentor-1)
- Live Site URL: [Live code](https://temitope15.github.io/frontend-mentor-1/)

## My process

- Created a parent container
- Created a card div
- Added my contents into the image parent and text parent divs
- created root colors
- centered my div with relative property on the parent , then top  and left 50% on the child container with the absolute property.
-did final styling to the text by centering it. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

I learnt how to center a div using the transform translate css property. I was able to center it both vertically and horizontally. I also learnt how to write a readme.md file.

To see how i used it, see below:


```css
.parent {
  position : relative;
}
.child {
  position:absolute;
  top:50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```
### Refactoring Process
- I decided to remove the transform translate property in my css file upon advice from a frontend mentor on Frontend mentor (https://www.frontendmentor.io/) to use the flex box model.
- So this is what i did to center my div
  ```css
  .parent {
    /*give the parent element a 100vw and 100vh*/
  width: 100vw;
  height:100vh;

  /* Then apply flex to center*/
  display: flex;
  align-items:center;
  justify-content: center;
  flex-direction:column;
  gap:10px;
  }
  .card{
    /* major styling */
  width: 250px;
  background-color: var(--whiteColor);
  padding: 10px;
  border-radius: 10px;
  /* to center the children elements */
  display: flex;
  flex-direction: column;
  align-items: center;
  }
  ```

  - I also updated the font to the font recommended in the style guide. I used google fonts.

  **How to use google fonts**
  ```html
  <!-- copy the link to the font you want from font.google.com -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Outfit&display=swap" rel="stylesheet">
  ```
   ```css
   /* use the style rules in the element you wish to use it*/
    body{
        font-family: 'Outfit', sans-serif;
        }
   ```
### Useful resources

- [Major Resource](https://www.freecodecamp.org/news/how-to-center-anything-with-css-align-a-div-text-and-more/) - This blog post helped me to be able to center my div using the transform translate css property.
- [W3Schools](https://www.w3schools.com/css/css_font_google.asp) - Here i learned how to use the google font in my code

## Author

- Frontend Mentor - [@Temitope15](https://www.frontendmentor.io/profile/Temitope15)
- Twitter - [@Sun_MadeCodes](https://www.twitter.com/Sun_MadeCodes)




