# Exercise 8: Adapting Bootstrap

OK, now it's time to try something really challenging.

Let's use Bootstrap to implement [a design we've worked on before](https://www.figma.com/file/SC3HqLUP9hGBfn93mIwxkS/Sports-App-homepage-Responsive-Revised).

Remember the Sports App? Let's implement the header and masthead from that design, but by using Bootstrap.

1. Add an `app.html` to your root folder.
1. Link up your `manifest.css` stylesheet.
1. Choose the right components from Bootstrap. Add Bootstrap compatible HTML to your `app.html`. Make sure the relevant components have their `@import`s enabled in `_bootstrap-manifest.scss`.
1. Add any custom components you might need.
1. The design is going to have a lot of custom values that don't match our Bootstrap values. Use approximate values by changing your bootstrap variables in a new variables file: `_bootstrap-app.scss`. This file will replace the `@import` in your `_bootstrap-manifest.scss` file.
