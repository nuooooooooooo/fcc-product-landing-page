# fcc-product-landing-page
My product landing page project from the FreeCodeCamp curriculum

For the overall design, I was inspired by this [codepen](https://codepen.io/Fizrook/full/NWqbgZL).

For the hamburger menu, I replicated [this tutorial](https://code-boxx.com/simple-responsive-pure-css-hamburger-menu/).

For the line appearing on hover under my name, I was inspired by the technique used in [this video](https://www.youtube.com/watch?v=djbtPnNmc0I). For future reference, to make the line expand, css can be written like this : 
```css
a::after {
  content: "";
  border-bottom: 2px solid white;
  position: absolute;
  top: 20px;
  left: 0;
  right: 0;
  bottom: 0;
  transform: scale(0, 1);
  transition: all 200ms ease-in-out;
}

a:hover::after {
  transform: scale(1, 1);
```

- Here is how `transform:scale` works as based on the video linked above. the first digit means the border has a width of 0% on the main axis, while it has a width of 100% on the y-axis. For the hover pseudo-element, setting them both to 1 makes it so they both have 100% width.
