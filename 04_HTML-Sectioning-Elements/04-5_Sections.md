# Sections

The difference between a section element and an article element can be somewhat confusing to being with. All you need to bear in mind is if you took that area of content away from it's surroundings - outside of the webpage - would it still make sense standalone?

If so it's probably an article, if not you probably want to use a section. You can have sections of articles or footers, or in fact sections of sections. Whatever makes sense to the content of that page.

Let's add a section to our article so you can see one being used:

```html
<article>
	<header>
		<h2>About</h2>
	</header>

	<p>This is about this website</p>

	<section>
		<h3>Get in Touch</h3>

		<p>You can get in touch here</p>
	</section>

</article>
```

You mgith also have a seciton which is by itself, but not standalone, so an article doesn't make sense:

Or a section within the footer for example: