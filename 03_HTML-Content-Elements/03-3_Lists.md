# Lists

Another common set of content elements are lists. There are three types of lists in html. The first is an unordered list, which we write by typing ul:

`<ul></ul>`

The unordered list has another element directly inside it, a _list item_ we type that with li:

`<li></li>`

An li tag is the only thing that can be a direct child of a ul, you can not use any other elements as direct children of an unordered list.

So you might create a list like this:

```html
<ul>
	<li>First list item</li>
	<li>List item two</li>
</ul>
```

Notice how the browser adds bullets to our list, because it knows it's a list.

The second type of list is an ordered list. This is exactly like an unordered list, we're just specifying this list _has_ order. Like chapters in a book. The browser isn't going to muddle up the order of the previous unordered list, but it will know that this ordered list should be in the order specified.

We write an ordered list with an ol:

`<ol></ol>`

Just like the unordered list, an ordered list's direct children can only be list items:

```html
<ol>
	<li>First list item</li>
	<li>List item two</li>
</ol>
```

See how the browser here puts numbers next to the list instead of bullets. We can change all these styles with CSS later.

The third list is a description list and this is different. This is written with a dl:

`<dl></dl>`

Inside this list you can have two elements. One for the term and one for the description. The term is a dt element:

`<dt>Term here</dt>`

The description is a dd element:

`<dd>Description of the term here</dd>`

You can actually have more than one term or more than one decription if you need to, you just have to remember to get the order right:

```html
<dl>
	<dt>Ultimate</dt>

	<dd>most important, highest, last, or final</dd>
	<dd>the best, most, or greatest of its kind</dd>
	<dd>last in a series</dd>
</dl>
```

