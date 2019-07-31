# Navs

One common element you might find on a page is a navigation: Links which take you to other places with a site or app.

There's a nav element to encapsulate that content.

`<nav></nav>`

Usually when we write the links (or anchors) inside our navigation we put them inside a list element. This isn't absolutely necessary so either of the following are completely valid.

```html
<nav>
	<a href="">Home</a>
	<a href="">About</a>
	<a href="">Contact</a>
</nav>
```

Or this:

```html
<nav>
 	<ul>
 		<li><a href=""></a></li>
 		<li><a href=""></a></li>
 		<li><a href=""></a></li>
 	</ul>
</nav>
```

You can also have other content in a navigation element:

```html
<nav>
	<h2>Primary nav</h2>
 	<ul>
 		<li><a href=""></a></li>
 		<li><a href=""></a></li>
 		<li><a href=""></a></li>
 	</ul>
</nav>
```

Any navigational content on the page can be wrapped in a nav element.