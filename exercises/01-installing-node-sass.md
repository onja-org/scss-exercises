# Exercise 1: Installing `node-sass`

Let's get `node-sass` working on this project.

We're going to use our compiled CSS to style the `index.html` in the root of this repo.

1. Install `node-sass` as a development dependency.
1. Commit your changes
1. Add a node script called `scss` that generates the CSS from the input `scss` folder to the output `css` folder.
1. Add another script that does the same, but additionally watches the `scss` folder for changes, triggering a `node-sass` compile each time the SCSS files change. Call this script `scss:watch`
1. Run your new scripts, and check [../index.html](your `index.html`) file. Does everything look OK?
1. With your `scss:watch` script running…
   1. Clear out the `.no-sass` selector in `manifest.scss`
   1. Delete the `<div class="no-sass">` node from `index.html`
   1. Delete the `<link>`ed stylesheet to `error.css` in `index.html`
1. Did Sass update the `manifest.css` file? If so: commit again. Your commit should include:
   - `scss/manifest.scss` changes
   - `css/manifest.css` changes
   - `index.html` changes
   - `package.json` changes
   - `package-lock.json` (new file)
1. Push