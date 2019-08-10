# Backgrounds

Being able to colour backgrounds for you elements, or add an image is very common when adding styles to your HTML. There's lots of CSS properties to enable you to do this.

Let's start with a simple background colour. This ones straight forward - it's just `background-color`, and now we know our colour values we can use any of those:

```css
p {
	background-color: #35af63;
}
```

But sometimes we might want an image as well. This property is background-image:

```css
p {
	background-color: #35af63;
	background-image: url('image.jpg');
}
```

<!-- need a background image that's too small so it repeats -->

We've kept the colour there as well, for a couple of reasons. Images need to be fetched from the server when you load a web page and this can take time, colours do not, so we're at least displaying something for the user whilst the image is loading.

You'll notice the image is duplicating itself across the element. That's because there is also a `background-repeat` property, which by default is set to `repeat`. Let's set it to `no-repeat` so we only have one image:

```css
p {
	background-color: #35af63;
	background-image: url('image.jpg');
	background-repeat: no-repeat;
}
```

The background image is positioned at the top and left of our _box_ (the element) by default. We can change that too. Let's use the background-position property. This can take two values, one for the horizontal position (x-axis) and one for the vertical position (y-axis), or we can use one value which is used for both.

```css
p {
	background-color: #35af63;
	background-image: url('image.jpg');
	background-repeat: no-repeat;
	background-position: center;
}
```

We can use words like `top`, `bottom`, `left` and `right` or unit values like `100px` (SHOW)

Let's use center.

It's still too small for the element. There's a `background-size` property, so we can use that to make the image bigger and fill our element. We can set the size with a unit, like pixels:

```css
p {
	background-color: #35af63;
	background-image: url('image.jpg');
	background-repeat: no-repeat;
	background-position: center;
	background-size: 100px;
}
```

But we need to know the precise measurements for out box, and they might be different to our image. There's also some keywords we can use to get the image to fill the box. You can write `contain`, `cover` or `auto`. Let's take a look and see what each do.

```css
p {
	background-color: #35af63;
	background-image: url('image.jpg');
	background-repeat: no-repeat;
	background-position: center;
	background-size: contain;
}
```

Contain keeps the whole image in the box, auto scales to the largest x or y size, and cover fills the box leaving no space. Let's use cover.

Just like `border` background comes with a shorthand. So we can write all these properties in one way, we write `background` instead of teh amended versions and put all the values in a space seperated list afterwards.

```css
p {
	background: #35af63 url('image.jpg') no-repeat center contain;
}
```

Order doesn't matter apart from size, which has to come after position. So keeping this order makes sense.