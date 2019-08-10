# Display Types

Before we get into setting dimensions and positioning our elements on our page, we need to understand how they work within the page by default.

We've already seen that browsers apply styles to elements, this is actually quite important when it comes to how we lay things out, because depending on what element it is and where is is within our HTML, depends on how it will behave when we try to size or move it.

Elements come with _default_ display types. These are as per the specification of the element itself and so browsers by and large implement it the same. If we are using our reset or nomalise this will help make sure they are the same.

Let's use our HTML page to look at what the display types are for certain elements

... inspect elements ...

We can see when we hover over these elements, they have a blue box showing the space they take up on the page. The display type for our sectioning elements (article, header, paragraph) are all `display: block`. The elements within the text and `display: inline`.

It's easy to visually see the difference between these two display types, because the _blocks_ fill all the space widths wise and sit on top of each other. The _inline_ elements take up as much space as the content within them and sit next to each other on the line. It's important to know what each of the elements are when we start to position them so if you're unsure just have a look with devtools.

There are other display types too - if we look at the lists we can see each item is a `list-item` display type. The `table` has specific display properties for the table and the cells, meaning each cell can exand to fit the content.

Have a look around the page and see which ones you can come up with.

As with all properties, we can set them ourselves with CSS. So if something is display inline, like this anchor here

...

We can set it to `display: block` 

```css
a {
	display: block;
}
```

See how that's made the links in the page take up the width space and be like a box, just like the article and header... This is a really important property to change and understand what it is doing when it does change.

One more thing before we move on to seeing how these display types affect other properties, there's also a value of `none` you can use with `display` - this removes the element visually altogether.

```css
a {
	display: none;
}
```

See how it's not there anymore and neither is the space for it.

If you wanted to keep it within the page, just _hide_ it there are a couple of different methods, there's a visibility property:

```css
a {
	visibility: hidden;
}
```

Or more commonly used these days because it's animatable, which is more the use case for keeping it there but not showing it, is the opacity property, which if set to 0, makes the element see through

```css
a {
	opacity: 0;
}
```

Let's move on to see how these display types affect other properties in CSS.