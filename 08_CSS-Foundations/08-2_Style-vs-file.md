# Style vs File

Let's talk about how to include your CSS within your HTML, so it affects your webpage.

There are a few ways to do this. The one that is used professionally is to include all your CSS in a seperate file and put a link to that file within the `head` element of your html, like so:

`<link rel="stylesheet" type="text/css" href="styles.css">`

There are a few attributes on teh `link` element, the first is the `rel` attribute, which defines the relationship to the html, in this case the link is a stylesheet. The second is the file type, which is a css file, so we have `type/css` in here. The third and most important is href, you remember the hyperlink reference we add to anchor elements in our HTML, this is the same, it's the path to the css file.

So if we were to create a `style.css` file, we would write the link to it here.

<!-- relative and absolute filepaths -->

In our css file, we can now write CSS, as we saw in the previous video.

This is the preferred way to do it, it keeps the CSS seperate, so it's easy to manage and it means we can share CSS between HTML pages. THis is the way we will be writing CSS for the rest of the course, however there are a couple more ways.

We can include CSS directly within the `head` of our HTML file. So within the `head` tags we write `style` tags and put CSS in there:

```html
<style>
	p {
		background-color: red;
	}
</style>
```

This is pretty fast as it loads with the HTML page, however it only works on the HTML page it's written on, which means when you are writing the CSS for a whole website it's not a great option as so much is shared.

The third way, which is reserved for special situations, is the `style` attribute. Which is added specifically to an element, so we don't need to write what we call a whole block of CSS but just the property and value pairs:

```html
<p style="background-color:red;">A paragraph</p>
```

As it's added directly to the tag, it just affects that one element and nothing else on the page. It also holds a lot of _weight_ even more than an ID - if you remember from our last video. This way of adding css is very specific.

For those reasons, we reserve it for interactive CSS changes, like those we would make with javascript.

Let's have a look at devtools again. If we look at our paragraph and the style panel, you will notice how the `style` attribute is first and affecting our element.

Let's stay in devtools and have a look around at the other styles that are on this paragraph. They are listed as you scroll down this style panel.

We haven't written any other CSS apart from what you see, but there's all this other CSS being applied. If we look next to each block it tells us _where_ the CSS is written, so all the methods we've just seen - the attribute, within style tags, or in a file - we can see. That means we can find the CSS if we need to.

However these other styles say they are from the user agent stylesheet. That's not something we have done, if you see this that means it's CSS that is being applied by the browser itself.

Remember when we were writing all our HTML and our headings were of different sizes, but we hadn't written any CSS yet. That's because the browser has default styles for all HTML elements.

Before we start writing CSS of our own we should either remove this styling, or look at ways to make sure all browsers have the same, as they all have their own unique styling.

Luckily for us some clever people before us have already thought of this. There's a solution for each situation, you just have to choose which one you want.

To strip all the styles, there's reset.css by Eric Meyer. It's some css which you can copy either into a file, or at the top of your css which removes the majority of browsers styles.

Or to make them all the same there's normalize.css, there's more CSS involved in this, so you need to include the file in your website.

