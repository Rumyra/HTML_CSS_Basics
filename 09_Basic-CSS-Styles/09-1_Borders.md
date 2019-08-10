# Borders

Let's start by taking a look at how to add a border to an element with CSS.

There are three properties: `border-style`, `border-width` and `border-color` The style is set with a specific value, things like solid, dotted. you can find a list here:

The width takes a unit value, before we go over unit values in depth let's use pixels, as they're pretty straight forward. You write them as a number and a `px` afterwards. This property determines how thick you want the border to be.

The `border-color` property sets the colour of the border and takes a colour value, which we will look at in more depth in the next chapter.

All of these properties set a border around the whole element.

```css
header {
	border-style: solid;
	border-width: 2px;
	border-color: black;
}
```

If we want to set just one side, rather than all around our element, we amend the property with the side: `top`, `bottom`, `left` or `right` like so:

```css
header {
	border-style-right: solid;
	border-width-right: 2px;
	border-color-right: black;
}
```

This will put our black border on just the right side.

This seems like a lot of CSS to write, especially if we want to put different borders on different sides.

In CSS we have a concept called shorthand, it means some properties can be written in a shorter way. We can just write `border` instead of all these different things, like style and width, and put them in a space seperated list after, like this:

```css
header {
	border: 2px solid black;
}
```

This gives us exactly the same thing as all our properties before, we just put all the values in our one property `border` rather than each of them.

We can do that with each side as well.

```css
header {
	border-top: 1px dotted grey;
}
```

Before we move on to look at some more styles we can use on different elements, let's take a look at what we can use as a colour value.

