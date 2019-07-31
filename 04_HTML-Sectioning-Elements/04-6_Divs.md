# Divs

The div element is a sectioning element you can use if you just want to put a wrapping box around content, usually for stylistic purposes, when none of the other sectioning elements make any sense.

It could be one area of a section needs to be moved over to the right side.

```html
<section>
	<h2>Some images and some text</h2>

	<div>
		<img src="" alt="" />
		<img src="" alt="" />
	</div>

	<p>Some content here</p>
</section>
```

Here we can use the `div` element when we're writing css to move both images together (which we'll look at later), but it doesn't mean anything content wise to the browser. We describe this as having _no semantic value_.