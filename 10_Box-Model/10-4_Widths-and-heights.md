# Widths and heights

TODO add default is auto

Now we've seen different units we can use, let's take a look at making some elements a size we might want.

Having paragraphs go across the whole page width can make them hard to read, so let's add a width to them to make them smaller.

```css
p {
	width: 50%;
}
```

This has made them half of the width of the conatiner they are in. It's the width property and it takes a unit for it's calue. We could have used pixels or viewport units or ems if we wanted.

...

We need an example of height - but to say this:

There is a `height` property as well. This allows us to specify a height for elements. However this is rarely used, because the height of elements is dictated by the contents within them. If I put a height on the paragraph, and then resize the browser window, you can see teh text flows outside of the height and doesn't expand with it:

```css
p {
	width: 50%;
	height: 400px;
}
```

This means we are breaking the _flow_ of the page, which we don't want to do, we want to keep it in tact, because all screen sizes are different, we don't know what size this content will be viewed at.

There might be situations where you want an element to have a minimum height and then get bigger if the content does overflow. There's a `min-height` property.

```css
p {
	width: 50%;
	min-height: 400px;
}
```

This is the same as width, there's a min-width property, and as well as that there's a max-width and max-height property too.

This means something can't get bigger than what you define. So if we wanted to make sure the paragraph couldn't get wider than a certain amount, becase long lines of text become unreadable, we could set a max-width on it.

```css
p {
	width: 50%;
	min-height: 400px;
	max-width: 500px;
}
```

Now that we've seen width and height, let's move on to look at how they affect the margin and padding we've already seen.
