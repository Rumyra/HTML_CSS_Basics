# CSS Flexbox

As we saw in the last section, floats and display types are good for some occasions but they only take us so far.

Flexbox was introduced to distribute elements along one axis. The browser does the work for us here and what we do is specify where on the axis we want the element, in what order and with what spacing.

There's lots and lots of different properties for Flexbox. So much so we're going to dedicate a whole course to deep dive into it. For now let's go over teh basics.

To use flexbox, you need to set a brand new display type on the containing element. If we go back to our nav, you'll see our parent element for our list items is our ul, so let's set `display: flex;` on that.

```css
ul {
	display: flex;
}
```

This now means all the direct children elements (our `li`s) are being distributed by the browser. Let's set the direction. by default this is row, and what we want, but let's just see what happens if we change it:

...

We want to allow for space in-between the elements. The property we want for this is `justify-content`, we can get all the lis to be at the start

SHOW

at the end, in the middle, space around them... there's lots of this. The value we want is `space-between`.

One more thing, if the browser gets to small this nav is going to overflow, we aren't going to learn how to change the design yet, so let's make that nav wrap. For this we need the `flex-wrap` property, which we set to `wrap`:

...

Remember, this was just an introduction to flexbox. For a full in depth course checkout the flexbox course which you can find in our ultimate courses HTML and CSS bundle...