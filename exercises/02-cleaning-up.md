# Exercise 2: Cleaning up

OK, we have `node-sass` running, good job!

Let's clean up things a little to prepare our project for the next set of exercises, and to keep things organised.

1. If you're running any node scripts in your terminal, please cancel them.
1. Delete the CSS files in the `css` folder

Alrighty, once that's done, let's start splitting up our SCSS files.

1. Create a `variables/_index.scss` file in the `scss` folder. This new  file is going to act as a variables manifest, pointing to all the other variable files we'll need.
1. Move the variables from `manifest.scss` into their own new files: 
   - `scss/variables/_colours.scss`
   - `scss/variables/_fonts.scss`
1. Create two `@import`s in `variables/_index.scss` that import these new variables files.
1. Finally, import the new variables manifest file (`_index.scss`) into `manifest.scss`.

Let's check that everything worked. If you run the `node-sass` compile script called `scss` you created in exercise 1, it should still compile fine, right?

Your SCSS folder should look like this:

```
scss/
  - variables/
    - _colours.scss
    - _fonts.scss
    - _index.scss
  - manifest.scss
```
1. Delete all the other content in the `manifest.scss` file. This file should only have the one `@import` in it.
1. Lastly, commit and push your changes.

