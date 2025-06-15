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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![Screenshot of the product preview card component](./screenshot.png)

### Links

- [Github Repository](https://github.com/ffrosch/frontendmentor-product-preview-card)
- [Live URL](https://ffrosch.github.io/frontendmentor-product-preview-card/)

## My process

### Initial setup

Install dependencies

```shell
bun create vite my-project --template vue
cd my-project
bun install
bun install tailwindcss
bun install -d @tailwindcss/vite
```

Add this to `vite.config.js`

```ts
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
    plugins: [
        tailwindcss(),
    ],
})
```

Add `@import "tailwindcss";` to `src/style.css`

Add this to `package.json`

```json
{
    "scripts": {
        "dev": "bunx --bun vite",
        "build": "bunx --bun vite build",
        "preview": "bunx --bun vite preview"
    }
}
```

### Built with

Tech Stack: Bun, Vite, Vue, Tailwind

- Mobile-first workflow
- Flexbox
- Tailwind custom theme
- [Vue](https://vuejs.org/) - JS library
- [Vite](https://vite.dev/) - Build tool
- [Tailwind](https://tailwindcss.com/) - CSS framework

### What I learned

Tailwind 4 combined with the "Tailwind CSS Intellisense" extension for VS Code makes styling and creating custom utility classes a breeze. Such a delight!
Using Bun and Vue for such a small project is overkill for sure, but it's great to get more practice in quickly setting up a development environment.

## Author

- Website - [florianfrosch.de](https://florianfrosch.de/)
- Frontend Mentor - [@ffrosch](https://www.frontendmentor.io/profile/ffrosch)
