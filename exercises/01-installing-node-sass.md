# Exercise 1: Installing `node-sass`

Let's get `node-sass` working on this project.

We're going to use our compiled CSS to style the `index.html` in the root of this repo.

1. Install `node-sass` as a development dependency.
1. Commit your changes
1. Add a node script that generates the CSS from the input `scss` folder to the output `css` folder.
1. Add another script that does the same, but additionally watches the `scss` folder for changes, triggering a `node-sass` compile each time the SCSS files change.
1. Commit again, and push.
1. Run your new scripts, and check [../index.html](your `index.html`) file. Does everything look OK?