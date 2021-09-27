# Frontend Mentor - Base Apparel coming soon page solution

This is a solution to the [Base Apparel coming soon page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/base-apparel-coming-soon-page-5d46b47f8db8a7063f9331a0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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


## Overview
My third FE challenge.

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - The `input` field is empty
  - The email address is not formatted correctly

### Screenshot

![Compeleted design screen shots with errors to note](./design/complete)

### Links

- [Github URL](https://github.com/PhilJG/frontendmentor-base-apparel-)
- [Live Site](https://philjg.github.io/frontendmentor-base-apparel-)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Vanilla JS

### What I learned

I reninforced my learnings around background image and gradients as well as form adjustment and validation...
```css
.btn {
    background-image: linear-gradient(to right, hsl(0, 80%, 86%) 5%, hsl(0, 74%, 74%) 100%);
}

```html
      <form id="form" action="#">
        <div class="input-box"></div>
          <input type="email" class="email-input" id="email" placeholder="Email Address" >
          <submit class="btn" id="btn" onclick="validation()"><span><ion-icon name="chevron-forward-outline"></ion-icon></span></submit>
          <span id="text"></span>
        </div>
      </form>
```js

function validation() {
        if (email.match(pattern)) 
        {
            form.classList.add("valid");
            form.classList.remove("invalid");
            text.style.color = "green";
            text.innerHTML = "Your Email Address is Valid";
            text.style.fontFamily = "Josefin Sans";
            text.style.fontSize = ".75rem";
            text.style.padding = "1rem";  
        }
        else 
        {
            form.classList.remove("valid");
            form.classList.add("invalid");
            text.innerHTML = "Please provide a valid email";
            text.style.color = "#ff0000";
            text.style.fontFamily = "Josefin Sans";
            text.style.fontSize = ".75rem";
            text.style.padding = "1rem";  
        }
}
```

### Continued development

I had trouble in these three areas:

- When the button is pressed the valid or invalid notice will come up. However it will not change if the text is change unless the page is refreshed. It seems that the function can only be called once?

- The blue border on the input box. Apparently when adjusted in :active or :focus states it does not change. How do I get rid of it?

- I`m having trouble with github pages. Whenever the button is pressed it just takes to a 404 page. That does not help demonstrate the work I did. How do I adjust this?

## Author

- Website - [philjgray.ca](https://www.philjgray.ca)
- Frontend Mentor - [@PhilJG](https://www.frontendmentor.io/profile/PhilJG)

