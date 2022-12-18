# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshots

Without any hovering: 

![Screenshot 2022-12-18 at 11 43 59](https://user-images.githubusercontent.com/102190049/208299071-e1cb9190-8403-4420-88c9-0f2ebdbadb38.png)

When you hover on the NFT image: 

![Screenshot 2022-12-18 at 13 16 46](https://user-images.githubusercontent.com/102190049/208299074-a5d60aa6-cfed-44f9-8d7f-7dee84a67c96.png)


When you hover on the tittle: 

![Screenshot 2022-12-18 at 13 17 04](https://user-images.githubusercontent.com/102190049/208299077-9bbd8944-83c6-46da-9497-2b5328c48635.png)

When you hover on the name: 

![Screenshot 2022-12-18 at 13 17 16](https://user-images.githubusercontent.com/102190049/208299079-6e161f3b-0ddb-49e1-8e89-27f615e9307e.png)



### Links

- Solution URL: [The Solution URL here](https://piouscode.github.io/NFT-Preview-Card-Component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

1. I learn how to add hover states to images with another image stack on top of it. 
2. I learn effective ways to position elements in the center of a particular container of the viewport in general. 


```html
<!-- Given the following html code, you can see how I play with different positioning techniques to get the desired result. -->

<div class="container">
  <div class="mainImage">
    <img
            class="diamond"
            src="images/image-equilibrium.jpg"
            alt="NFT Equilibrium Photo"
    />
    <div>
      <img
              class="diamond"
              src="images/icon-view.svg"
              alt="View Icon"
      />
    </div>
  </div>

```
```css
/* In this CSS code you can see how I play with the different positioning techniques to achieve the objective of this challenge */


.mainImage {
  position: relative; /* Set position to relative */
  padding: 24px; /* Set padding */
}

/* Set styles for the diamond class */
.diamond {
  width: 302px; /* Set width */
  height: 302px; /* Set height */
  border-radius: 8px; /* Set border radius */
}

/* Set styles for div elements within mainImage class */
.mainImage div {
  position: absolute; /* Set position to absolute */
  background-color: hsl(178, 100%, 50%, 60%); /* Set background color */
  top: 0; /* Set top position to 0 */
  width: 302px; /* Set width */
  height: 302px; /* Set height */
  margin-top: 24px; /* Set margin */
  opacity: 0; /* Set opacity to 0 */
}

/* Set styles for div elements within mainImage class when hovered over */
.mainImage div:hover {
  opacity: 1; /* Set opacity to 1 */
  cursor: pointer; /* Change cursor to pointer */
  border-radius: 10px; /* Set border radius */
}

/* Set styles for img elements within mainImage div elements */
.mainImage div img {
  position: absolute; /* Set position to absolute */
  top: 50%; /* Set top position to 50% */
  left: 50%; /* Set left position to 50% */
  transform: translate(-50%, -50%); /* Center the element */
  width: 48px; /* Set width */
  height: 48px; /* Set height */
}
```


### Continued development

Now, my primary objective is to comprehend the function of each element and property. I like to have a greater grasp of why things function the way they do as opposed to having to guess. This is my next challenge, hoping that with these little challenges from the frontend mentor, I am able to reach my goal as quickly as possible.

## Author

- Github Profile - [Piouscode](https://github.com/Piouscode)
- Frontend Mentor - [@Piouscode](https://www.frontendmentor.io/profile/Piouscode)


