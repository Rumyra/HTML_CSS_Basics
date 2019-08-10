# Box Shadows

One last bit of styling before we move on. We can add borders and background to our elements, but we can also add a shadow around the edge.

We do this with the `box-shadow` property. There is no long or shothand for this, it's just one set of values - let's take a look:

```css
p {
	box-shadow: 1px 1px 1px 1px grey;
}
```

The numbers are as follows. The first is the shadow on the horizontal, so a positive goes right, a negative goes left, let's see what 0 will do...

The second is the vertical and the same applies (increase val, negative).

The third is how much blur there is. Let's see what happens when we change it.

...

The forth is what we call spread, which is where the blur starts from, so making this bigger makes the box look more raised.

...

Now that we've had an introduction to some styles with CSS, and got used to it. Let's take a look at the beginnings of understanding layout, changing size of things and moving things around.