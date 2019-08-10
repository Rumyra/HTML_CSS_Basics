# Units

There's lots and lots of different units you might use in CSS. Here we'e going to cover common ones you will use and see when you're writing CSS.

We've already seen pixels. Screens are displayed in pixels, so this unit makes sense in that one pixel in CSS represents one pixel on a screen. One pixel is pretty small:

```css
p {
	border: 1px solid red;
}
```

If I make that border 10px it will be thicker, because it will be 10 pixels thick

```css
header {
	border: 10px solid red;
}
```

This is a good all round unit, and you can use any numeric value in here, like it could be 900 pixels!

However, all the screens out there are different sizes, and you don't know how big the screen is that the user who viewing your website is using. It might be a small phone screen or a big tv. So this isn't a good unit for using to size the elements on your page, because it's what we call an _absolute_ unit, it's the same on all screens, regardless of how big the browser is. That means if teh browser is small, the element could overflow.

```css
header {
	border: 10px solid red;
	width: 900px;
}
```

We've added a width to this header (we'll talk more about widths in the next section). But for now all we need to know is that you set them with a unit. Here 900p is too big and it goes beyond the screen we're viewing it on.

A better unit for this is a percentage. This takes into account the parent element, and takes a percentage from that, so in this case, the whole width of the browser, if we set the header to half - 50%, it will be half the width:

```css
header {
	border: 10px solid red;
	width: 50%;
}
```

That's much better, because if we change the size of the browser, the header changes too. THat means it doesn't matter how big the browser is, the header will always take up the same amount of space.

We call this a _relative_ unit.

There are some other _relative_ units which are also good. Because percentage takes into account the parent element, we might always want it to take into account the browser. We have viewport units, which are a part or the viewport. 1% actually.

There's viewport width, which we write as `vw`, which is one percent of the viewport width:

```css
header {
	border: 10px solid red;
	width: 50vw;
}
```

This is the same as percentage, but won't be affected if we change the element above it.

EXAMPLE

There is also viewport height, which is one percent of the viewport height, rather than width. This can be handy if we want an app to fill the whole height of something:

It's worth noting, these are just units, we can use them wherever a unit value is valid, so I could use the viewport height unti int eh width here:

```css
header {
	border: 10px solid red;
	width: 60vh;
}
```

Aswell as viewport height and viewport width, there's a viewport max (vmax) and viewport min (vmin) these change depending on which of vw or vh is bigger or smaller. If vw is biggest, one of those is set to vmax, otherwise if vh is bigger, is one viewport height unit. Conversly it's the opposite for vmin. If one viewport width is smaller, that is what is set as the vmin mesure. We use them the same as vh and vw:

```css
header {
	border: 10px solid red;
	width: 50vmin;
}
```

There's some mesurements which are specific to fonts, even though they are units and we can use them whereever we want.

The most common are em and rem. It's best to illustrate the difference between these two with an example.

One em unit is the equal to the current font size of the element. By default, unless changed by CSS, a web pages font size is 16px, however it is a style inherited by elements. So if it's 16px on the body, then a paragraph will be 16px as well. Pixels are aboslute values, so youw ouldn't notice a change, however an em is a relative value. So if if the body has an em size of 1.2em and a paragraph 1.2em, then the paragraph will have a font size of 1.2 times 1.2,

Let's look at an example.

```css
body {
	font-size: 1.2em;
}
p {
	font-size: 1.2em;
}
```

See how the paragraph is bigger than... this can be useful, as by and large designs are made by using a ratio when it comes to font sizing. However it can also be frustrating in web development, because you might come and add a different element within your HTML with a different font size and this could cause erratic behaviour.

Let's say an article also had 1.2 em.

```css
body, article, p {
	font-size: 1.2em;
}

```

The paragraphs inside articles are now even bigger!

This can be solved by using rem, which is root em and only takes a value from the root element. Which is the toppermost element. In our case html, ignores the other parent element - let's change our css:

```css
body, article, p {
	font-size: 1.2rem;
}

```

See how that's made all the paragraphs the same. This is much more stable when working with this kind of sizing unit.

These are the most common sizing units. There's a whole list of other ones, like mm or inches (which you might want to use in print). You can find a link to a list in the resources.