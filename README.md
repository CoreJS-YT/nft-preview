# Frontend Mentor - NFT preview card component

## Description

Aqui hise el reto de [**NFT preview card component**](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U/hub) terminado en (2 hrs)

## Commits

### **1 Commit( *Iniciando El Reto* )**

Los Archivos del reto

- NFT Preview
    - CSS
        - index.css
        - attribute.css
    - DESIGN
        - active-states.jpg
        - desktop-design.jpg
        - desktop-preview.jpg
        - mobile-design.jpg
    - IMAGES
        - favicon-32x32.png
        - icon-clock.svg
        - icon-ethereum.svg
        - icon-view.svg
        - image-avatar.png
        - image-equilibrium.jpg
    - .gitignore
    - index.html
    - README-templeate.md
    - README.md
    - style-guide.md

### **2 Commit( *HTML Terminado* )**

Este es el codigo que use en el html

```html
<main class="card">
    <div class="card__preview">
      <img src="./images/image-equilibrium.jpg" alt="Image NFT" class="card__preview__image">
    </div>
    <div class="card__description">
      <h1 class="card__description__title">Equilibrium #3429</h1>
      <p class="card__description__desc">Our Equilibrium collection promotes balance and calm.</p>
      <div class="card__description__date">
        <p class="card__description__date__price"><img src="./images/icon-ethereum.svg" alt="Etheruem"> 0.041 ETH</p>
        <p class="card__description__date__time"><img src="./images/icon-clock.svg" alt="Time"> 3 days left</p>
      </div>
    </div>
    <div class="card__creator">
      <img src="./images/image-avatar.png" alt="Image Avatar" class="card__creator__avatar">
      <p class="card__creator__name"> Creation of Jules Wyvern</p>
    </div>
  </main>
```

### **3 Commit( *CSS Terminado* )**

Este es el codigo que utilize en el archivo css

```css
:root {
    /* Font */
    --font-Outfit: 'Outfit', sans-serif;
    /* Colors */
    /* Primary */
    --Soft-Blue: #8bacda;
    --Cyan: #00fff7;
    /* Neutral */
    --Very-Dark-Blue-main-BG: #0d192b;
    --Very-Dark-Blue-Card-BG: #14253d;
    --Very-Dark-Blue-line: #2f415b;
    --White: #ffffff;
}
* {
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}
body {
    font-size: 18px;
    font-family: var(--font-Outfit);
    background-color: var(--Very-Dark-Blue-main-BG);
}

.card {
    background-color: var(--Very-Dark-Blue-Card-BG);
    width: 320px;
    height: 540px;
    overflow: hidden;
    margin: 50px auto;
    border-radius: 12px;
}
.card__preview,
.card__preview__image {
    width: 280px;
    height: 280px;
    border-radius: 12px;
    margin: 10px 10px 30px 10px;
}
.card__description {
    width: 320px;
    height: 140px;
}
.card__description__title {
    color: var(--White);
    font-weight: 600;
    font-size: 1.10em;
    margin: 0px 15px 10px 20px;
    transition: all .3s;
}
.card__description__title:hover {
    color: var(--Cyan);
    cursor: pointer;
}
.card__description__desc {
    color: var(--Soft-Blue);
    font-weight: 300;
    margin: 0px 15px 10px 20px;
}
.card__description__date {
    display: flex;
    justify-content: space-between;
    margin: 0px 20px 0 20px;
}
.card__description__date__price {
    color: var(--Cyan);
    font-weight: 600;
}
.card__description__date__time {
    color: var(--Soft-Blue);
    font-weight: 600;
}
.card__description__date__price,
.card__description__date__time {
    display: flex;
    text-align: center;
    align-items: center;
    gap: 5px;
}
hr {
    margin: 0px 20px;
    display: flex;
    align-items: center;
    border: 1px solid var(--Very-Dark-Blue-line);
}
.card__creator {
    width: 320px;
    height: 17px;
    display: flex;
}
.card__creator__avatar {
    width: 36px;
    height: 36px;
    margin: 15px 20px;
    border-radius: 100%;
    border: 1px solid var(--White);
}
.card__creator__name {
    display: flex;
    align-items: center;
    color: var(--Soft-Blue);
    font-weight: 400;
    font-size: .98em;
    margin: 23px 20px 23px 10px;
    width: 195px;
    height: 20px;
    text-align: center;
    letter-spacing: .15px;
}
span {
    color: var(--White);
}
@media (min-width: 700px) {
    .card {
        margin: 90px auto;
    }
}
```