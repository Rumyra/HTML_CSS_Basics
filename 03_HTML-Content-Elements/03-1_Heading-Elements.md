# Heading Elements

We'll split the different HTML elements we're going to cover into their own videos for you, so if you need to refer back to an individual element you can easily do so.

All the elements we'll be looking at from now on in the HTML section of this course are elements we write within the `body` tag of the document we created. Go ahead and open the `index.html` file that comes with this part of the course and we can start from where we left off.

There's a lot of text content on web pages and in apps. Let's start with the headings you might come across in different parts. Whether that be the overall heading of the website, a blog post heading, or a status update heading. They are all depicted by these heading tags.

The elements themself all start with h and end with a number - from 1 through to 6, depending on the weight of the heading on the page. So for the top titale of the site, we would use an h1:

`<h1></h1>`

And inside this tag we would put the title of the site:

`<h1>My Cool Site</h1>`

If we needed a heading for an article within the page, we could use another level of heading, like an h2.

`<h2>An Article Heading</h2>`

And if that article has sub headings we could use yet another level:

`<h3>Article Sub Heading</h3>`

It's also worth noting here you can have more than one of these headings per page. You may have two articles, in which case the headings for both of these articles carry the same weight and should both use the h2 level.

An example of how you would structure these headings might be something like:

```html
<h1>My Cool Site</h1>

<h2>An Article Heading</h2>
<h3>An Article Sub-heading</h3>
<h3>Another Article Sub-heading</h3>

<h2>Another Article</h2>
<h3>Sub-heading</h3>
```

And so on and so forth. You have up to h6 for your levels. You notice that these headings have different sizes, these sizes are added to the browser by default, but we can change them later with CSS, so you should always keep in mind the order of the headings, not the size of them in any design of the webpage. The order is more important.