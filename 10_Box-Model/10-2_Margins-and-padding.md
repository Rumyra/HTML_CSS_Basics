# Margins and Padding

At the moment, all the space in and around are elements has been set by the browser, and we have either reset it, or made it the same with normalise. It's not going to be the same as the design we're trying to create.

There's two properties for space _inside_ an element and space _outside_ an element.

Space _inside_ an element is padding. We set it with the padding property:

```css
article {
	padding: 10px;
}
```

It takes a unit value. This code puts 10px of space on the inside of our article. If you remember our border property, we could set our border on any one of our sides. We can do this with padding too. We can put it at the top, bottom, left or right: What we have written above is our shorthand and is the equivilant to:

```css
article {
	padding-top: 10px;
	padding-right: 10px;
	padding-bottom: 10px;
	padding-left: 10px;
}
```

So we could set different spacing:

```css
article {
	padding-top: 10px;
	padding-right: 20px;
	padding-bottom: 30px;
	padding-left: 40px;
}
```

We could do this with our shorthand as well, by writing four values one after the other:

```css
article {
	padding: 10px 20px 30px 40px;
}
```

To remember the order of the values, they start at the top of the box and go clockwise. So the first value is top, the second is right, the third is bottom and the forth is left.

There's a couple more shorthand versions. You can put in two values and they account for the top & bottom and left & right:

```css
article {
	padding: 10px 20px;
}
```

Or three, which is top, left & right and bottom

```css
article {
	padding: 10px 20px 30px;
}
```

Don't worry if you don't remember all of them right away, just knowing they are there is good enough for now. We'll use them when we need to through out the course to refresh your memory.

If we want to put space on the _outside_ of an element, we use the `margin` property. It works exactly the same way as padding:

```css
article {
	margin: 10px 20px 30px 40px;
}
```

You can see, it's put space on the outside of the box as well.

The long hand properties are the same as padding, so we can write the above just like this:

```css
article {
	margin-top: 10px;
	margin-right: 20px;
	margin-bottom: 30px;
	margin-left: 40px;
}
```

or if we want it to be all the same, like this:

```css
article {
	margin: 10px;
}
```

Let's see what happens if we put space inside or outside an inline element, like this span inside our paragraph:

```css
span {
	background-color: pink;
	border: 1px solid green;
}
```

Let's put a background colour on and a border, so we can see what's happening.

```css
span {
	background-color: pink;
	border: 1px solid green;
	padding: 10px;
}
```

The padding gets applied as normal, with space inside the element, but watch as we apply margin:

```css
span {
	background-color: pink;
	border: 1px solid green;
	padding: 10px;
	margin: 10px;
}
```

The margin doesn't move the elements either side, if we inspect the element, we can see the margin is there, by this orange around the box. However this is behaviour we want as we want the element to stay _inline_ with all the other elements.

There is another display type we haven't mentioned yet. it's `inline-block` this gives us both features. It keeps the element inline, but the margin and padding is affected as we would imagine it to be.

```css
span {
	background-color: pink;
	border: 1px solid green;
	padding: 10px;
	margin: 10px;
	display: inline-block;
}
```

See how the span is now acting like a box in accordance with the margin and padding, but it's still staying inline with the text. It's a good idea to remember this display type as it could come in handy.

before we move on to look at how to change the size of our elements. Lets have a closer look at some unit values we might use in CSS in the next part
