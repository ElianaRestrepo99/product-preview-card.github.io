# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

-It is a template of a sales product made with html and css.

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./images/desktop.pngs)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

My process was very dynamic and pleasant, the development of this template dividing its content between an image and a div, plus the implementation of very beautiful neutral color styles giving elegance to the template.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">

  <link rel="stylesheet" href="./style.css">
  
  <title>Frontend Mentor | Product preview card component</title>

</head>
<body>

  <div class="container">
    <div class="grid">
      <div class="img">
        <img src="./images/image-product-desktop.jpg" alt="">
      </div>

      <div class="card-content">
        <h6 class="pro-cat"> Perfume</h6>
        <h2 class="pro-name"> Gabrielle Essence Eau De Parfum</h2>
        <p class="pro-des"> A floral, solar and voluptuous interpretation composed by Olivier Polge, 
          Perfumer-Creator for the House of CHANEL.</p>
          <div class="price">
            <p class="current-price"> $149.99</p>
            <p class="old-price">$169.99</p>
          </div>

          <button class="cta">
            <img src="./images/icon-cart.svg" alt="icon-cart">
            Add to Cart</button>
      </div>
    </div>

    <div class="attribution">
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
      Coded by <a href="#">ElianaRestrepo99</a>.
    </div>
  </div>


</body>
</html>

```
```css
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,100..900;1,9..144,100..900&display=swap');


*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    font-family: 'Montserrat',sans-serif;
    background-color:hsl(30, 38%, 92%);
    font-size: 14px;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container{
    margin: 30px auto;
    padding: 0 30px;
}

.grid{
    max-width: 700px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    background-color: #fff;
    border-radius: 15px;
    overflow: hidden;
}

.img img{
    max-width: 100%;
    display: inherit;
}

.card-content{
    padding: 35px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

h6.pro-cat{
    text-transform: uppercase;
    letter-spacing: 3px;
    font-size: 13px;
    color:  hsl(228, 12%, 48%);
    font-weight: 500;
}

h2.pro-name{
    font-family: 'Fraunces',serif;
    font-size: 34px;
    line-height: 1em;
    color: hsl(212, 21%, 14%);
}

p.pro-des{
    color: hsl(228, 12%, 48%);
    line-height: 1.6em;
}

p.current-price{
    font-family: 'Fraunces, serif';
    color: hsl(158, 36%, 37%);
    font-size: 25px;
    padding-right: 25px;
}

.price{
    display: flex;
    align-items: center;
}

p.old-price{
    color: hsl(228, 12%, 48%);
    text-decoration:line-through;
}

button.cta{
    background-color: hsl(158, 36%, 37%);
    border: none;
    padding: 12px 0;
    border-radius: 14px;
    color:  hsl(0, 0%, 100%);
    font-size: 14px;
    font-weight: 700;
    cursor: pointer;
    transition: background-color .6s ease;
}

button.cta img{
    padding-right: 7px;
}

button.cta:hover{
    background-color:hsl(158, 36%, 23%);
}



    .attribution {
         font-size: 11px;
         text-align: center; 
         color: brown;
        }

    .attribution a {
         color: hsl(228, 45%, 44%);
         }

```
```js
const proudOfThisFunc = () => {
  console.log('🎉')
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
