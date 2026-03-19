# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_snu9D). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [My Workflow](#my-workflow)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### Screenshot

![Design preview for the QR code component card](https://thecoder-rahul.github.io/fontend_mentor_qr_code/thecoder-rahul.github.io_fontend_mentor_qr_code_.png)

### Links

👉 Solution URL: [Add your GitHub URL here](https://github.com/TheCoder-Rahul/fontend_mentor_qr_code)
👉 Live Site URL: [Add your GitHub Pages URL here](https://thecoder-rahul.github.io/fontend_mentor_qr_code/)

## My process

### Built with
- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### My Workflow
1. **Analysis**: Studied the design images to define the container-child relationship.
2. **Structure**: Built the card using a `<section>` tag for the card and `<img>`, `<h1>`, and `<p>` for content.
3. **Styling**: Imported font from the Google Fonts and applied global styles (colors/typography) then moved to layout positioning.
4. **Refinement**: Adjusted margins and padding to match the design "eye-ball" test.

### What I learned

The main challenge was ensuring the card stayed centered regardless of the viewport height. I solved this by using min-height: 100vh on the body. I also practiced using relative units (like rem) for font sizes and padding to ensure better accessibility and scaling across different browser settings.

## Author

👉 Frontend Mentor - [@TheCoder-Rahul](https://www.frontendmentor.io/profile/TheCoder-Rahul)
👉 GitHub - [TheCoder-Rahul](https://github.com/TheCoder-Rahul)

```css
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@400;700&display=swap');
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Outfit', sans-serif;
}
body {
  height: 100vh;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  color: hsl(220, 15%, 55%);
  background-color: hsl(212, 45%, 89%);
}
.card {
  text-align: center;
  border-radius: 20px;
  width: min(320px, 90%);
  padding: 16px 16px 40px;
  background-color: #fff;
  box-shadow: 0 25px 25px rgba(0, 0, 0, 0.04);
}
.card img {
  width: 100%;
  border-radius: 16px;
  margin-bottom: 24px;
}
.card h1 {
  font-size: 22px;
  line-height: 120%;
  margin-bottom: 16px;
  color: hsl(218, 44%, 22%);
}
.card p {
  font-size: 15px;
  line-height: 140%;
  letter-spacing: 0.2px;
  color: hsl(216, 15%, 48%);
}
.attribution {
  font-size: 11px;
  text-align: center;
  position: absolute;
  bottom: 1rem;
}
.attribution a {
  color: hsl(228, 45%, 44%);
}
