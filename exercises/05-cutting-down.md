# Exercise 5: Cutting down Bootstrap

You might have noticed, our `manifest.css` file is HUGE now.

We don't need all the components we're not using right now, so lets see if we can figure out how to cut down Bootstrap to only provide for what we're using.

It starts by changing the way we import Bootstrap.

First, we're going to copy the way Bootstrap imports all its SCSS.

1. Create a `_bootstrap-manifest.scss` file in your `scss` folder.
1. Copy the contents of the real `bootstrap.scss` file (located at `node_modules/bootstrap/scss/bootstrap.scss`) and paste it into your new `_bootstrap-manifest.scss` file.
1. Change the URLs of all the `@import` rules in the new bootstrap-manifest file so that they reference their relevant files. (Each of those `@import`s used to reference sibling files in the `node_modules/bootstrap/scss/` folder. Now we're trying to reference them from our `scss` folder.)

Now, let's check that bootstrap is still working correct.

1. In your `manifest.scss` file, change the `@import` for `bootstrap` so that it uses our new bootstrap-manifest file.
1. Run your SCSS script, so that it compiles our CSS.

Resolve any errors you might have.

If that's all looking good, then **commit and push your work**.

Let's get a reading of how big the CSS is right now.

Open `form.html` in your browser. Using the browser devtools' Network tab, tell me how big is the `manifest.css` file, in terms of file-size?

Start your `scss:watch` script.

Alright, now comment out all the `@import`s in `_bootstrap-manifest.scss`, except for the first three.

In other words, you should only have 3 imports active:

```
@import "../node_modules/bootstrap/scss/functions";
@import "../node_modules/bootstrap/scss/variables";
@import "../node_modules/bootstrap/scss/mixins";
```

OK, tell me, how many kilobytes is the `manifest.css` file now?

Why is it that size? Shouldn't it be larger than that?

Alright, now start adding the various bootstrap components back by uncommenting the imports you'll need. e.g. you know you're going to need button styles, so make sure you import Bootstrap's button component.

Make sure the `form.html` page is still styled correctly. Keep adding individual components 

What file size in kilobytes is your CSS now?
How many `@import`s are you using now?

Once you've got everything working, **commit and push**.