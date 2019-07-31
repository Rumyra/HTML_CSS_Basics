# Main and aside

The main element represents the main, unique content of the web page or app. Being unique it can not include content which is repeated throughout the whole site or application, so excludes the main header and footer elements for example.

You can not have more than one main per html document. Let's use it to encapsulate our content we have written so far:

`<main></main>`
<!-- wrap around content -->

The aside element represents content which is indirectly related to that sections main content.

This could be a sidebar for the main content, or noted text within an article.

`<aside>Side bar here</aside>`

```html
<aside>
	<p>Some related text</p>
</aside>
```

On the face of it there are a lot of these sectioning elements, and because they don't show when we write them in html, it may be a bit strange to use them at the moment, but when we star tto use css they will become very valuable. And with practise you will learn all of them and which ones to use in the right places.