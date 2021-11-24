# Header Section
```html
.header>.header__logo-box+.header__text-box
```

```css
.header{
  height: 95vh;
  /* background image with linear gradient and image */
  background-image: linear-gradient(to right bottom, rgba($color-primary-light, 0.8), rgba($color-primary-dark, 0.8)), url(../img/hero.jpg);
  background-size: cover;
  background-position: top;
  /* four line at clockwise direction */
  clip-path: polygon(0 0, 100% 0, 100% 75%, 0 100%);
  position: relative;
}
```

```css

    &:hover {
      outline: 1.5rem solid $color-primary; 
      /* //create green outline   outline-offset: 2rem; at parent div */
      transform: scale(1.05);
      box-shadow: 0 2.5rem 4rem rgba($color-black, 0.5);
       /* //increase shadow at bottom */
      z-index: 20;
    }

    &:hover &__photo:not(:hover) {
    transform: scale(0.95);
    /* photo that are not hover and scale down */
  }

```