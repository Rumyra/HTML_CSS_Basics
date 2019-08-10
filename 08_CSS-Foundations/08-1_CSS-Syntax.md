# CSS Syntax

Before we start including some CSS aong side our HTML, let's have a look at the syntax. The way we _write_ CSS.

CSS comes in what we call property-value pairs. By that we mean we write two things at a time. We write the thing we want to style, and the way we want to style it.

Let's take a look at an example.

```css
article {
	background-color: red;
}
```

The first thing you'll notice is we have `article` written. This is the element we want to change the look of, this is called the selector. We'll come back to that in a minute, as there are a few ways to write this part.

After we've written the _selector_ we open curly braces, these encompass all the property value pairs we want to write for that element, so we must remember to type a closing one after we've finished!

In this example the _property_ we want to change on the element is `background-color`, it's pretty self explanatory, it will set the colour of the background. The _value_ we set here is `red`. Now each property allows it's own set of values, there are colour values, unit values, keywords you can use. Lots of different ones. Over this course we will visit most of them and discuss how to use them.

Let's take a look at what happens if we change the value:

```css
article {
	background-color: blue;
}
```

You can see the colour of the article background is now blue, not red.

Let's take a look at another example, not only can you set a background colour but you can also set a background image:

```css
article {
	background-color: blue;
	background-image: url('../iamges/bk.jpg');
}
```

Now you can see the article has an image as a background instead. I've kept the colour in too because if the image doesn't load for any reasons, or takes a while to load, we have a similar colour being shown in the meantime.

You'll see the `value` for the property `background-image` is slightly different than just a word. It uses url and then brackets, and then a path to an image. This is the url function. Whenever you see a word and brackets _directly_ afterwards in CSS, it's a function and will do soemthing special. In this case it's going to load the image for us.

Let's talk about that `article` part, the selector. This means the CSS is going to go to the HTML and find all the `article` elements and apply the CSS we write.

There are different selectors we can use, so here we have an element as a selector. We could have header, or h1, or p or any of the elements we saw in the previous chapter.

NB CHANGE SELECTOR AND SHOW BACKGROUND CHANGING

Another selector we could use is a class. A class is a common attribute we can use in HTML. We write it like this:

`<p class="lede">This is a bigger paragraph</p>`

You will see the attribute `class` on the element. We can use the class attribute on any element within the body and we can write whatever value we want in the class attribute. If we put a space in the value, we are putting two classes on the element:

`<p class="lede call-out">This is a bigger paragraph</p>`

This paragraph now has two classes, `lede` and `call-out`. We can use classes in CSS as a selector, but we have to remember to put a fullstop before the name:

```css
.lede {
	background-color: red;
}
```

You can see here I have used the `lede` class to make the background colour of the paragraph red. But I had to use a fullstop before writing the name of the class.

I could have used `call-out` instead.

```css
.call-out {
	background-color: red;
}
```

Another type of selector is an id. This is set on an HTML element as an attribute as well.

`<p id="feature">This is a feature paragraph</p>`

You use it in css just like a class, but instead of putting a fullstop before it you put a hash symbol.

```css
#feature {
	background-color: red;
}
```

You can use an id on any element, however you can't have any two id's the same, so I wouldn't be able to do:

`<article id="feature"></article>`

within the same HTML page. You _can_ do this with classes however. You can use a class multiple times, so this _is_ allowed:

`<article class="call-out"></article>`

For this reason id's carry what we call more _weight_ than classes, so we tend to use classes within css rather than ids.

Let's go back to the example with two classes on the same element (you can't have two ids, only one):

`<p class="lede call-out">This is a bigger paragraph</p>`

We've already seen that we can use either class, but what if your CSS contains both classes, as you start to write CSS you'll learn that this can be common.

```css
.lede {
	background-color: red;
}
.call-out {
	background-color: blue;
}
```

Because the paragraph has both classes on it, both those CSS styles are affecting it. Let's have a quick look, by opening the browser dev tools.

You can see in the styles panel here, both background colours are there. But the blue is over-ridding the red and being set on the paragraph. This is because it is written afterwards in our CSS.

By and large whatever is written last over-writes whatever is written further up in our CSS, apart from some special circumstances.

Different selectors carry different weights. If I had used the `p` element as my selector like so:

```css
p {
	background-color: blue;
}
```

This carries less weight than a class, so if I were to write this in my CSS:

```css
.lede {
	background-color: red;
}
p {
	background-color: blue;
}
```

Instead of it following the last gets applied rule, it's the class styling that affects the paragraph, because classes as a selector hold more _weight_ than elements do.

It's the same for id's, in fact, id's hold the most weight. Let's add an id to the paragraph as well as our classes:

`<p class="lede call-out" id="feature">This is a bigger paragraph</p>`

And then write an order something like this:

```css
.lede {
	background-color: red;
}
#feature {
	background-color: pink;
}
p {
	background-color: blue;
}
```

You can see the background color of the paragraph is pink, even though we haven't written it last. Because the id holds the most _weight_. If I move the id, it's still getting applied.

Don't worry if this is slightly confusing at this point. As we go through the CSS part of this course we'll do some excercises and practise and touch on this point again.

There's a couple more things to note about selectors. You probably have multiple paragraphs on a page, so if I used `p` as my selector, this is going to affect all paragraphs on my HTML page.

```css
p {
	background-color: blue;
}
```

They will all have a background of blue. This can actually be very useful, maybe not for backgrounds, but you can also style text with CSS, so you can give all the paragraphs the same font size for example. The property for font size, is font-size, with a hyphen.

```css
p {
	font-size: 1.2em;
}
```

The value here is a unit value, there are lots of unit values and we will cover them in the course. So all our paragraphs have the same font size.

However you might have a situation where you want one paragraph to have a bigger font size - this is where our classes come in useful:

```css
p {
	font-size: 1.2em;
}
.lede {
	font-size: 1.6em;
}
```

Now you can use a class of `lede` on any paragraph (or any other element in fact) and it will increase the font size from 1.2em to 1.6em

```html
<p class="lede">This is a bigger paragraph</p>
<p>This is a normal paragraph</p>
```

This is what we refer to as the _cascade_, depending on what selector you are using affects how many elements on the page you want to style, and you can get more specific as you work your way through. We'll see this in action with in this part of the course.

One last thing is styling more than one selector at a time, or elements within elements. Both of these can be done. Let's take a look.

Here's some HTML:

```html
<article class="feature">
	<p class="lede">This is a bigger paragraph</p>
	<p>This is a normal paragraph</p>
</article>

<p class="lede">Another paragraph</p>
```

We've seen how you could target all the paragraphs here, you could just use the `p` element as the selector:

```css
p {
	border-bottom: 1px solid grey;
}
```

This puts a grey border on the bottom of the paragraphs. But what if you wanted that on the article as well. Instead of repeating yourself like so:

```css
p {
	border-bottom: 1px solid grey;
}
article {
	border-bottom: 1px solid grey;
}
```

you can target two selectors at the same time by putting a comma in between them

```css
p, article {
	border-bottom: 1px solid grey;
}
```

And remember you can use any selector, so the classes we have on the paragraphs can be used:

```css
.lede, article {
	border-bottom: 1px solid grey;
}
```

But what is you wanted to just style the `lede` paragraph _inside_ the `feature` article. There's a way to do that as well. Instead of putting a common inbetween the selectors, you put a space.

```css
.feature .lede {
	border-bottom: 1px solid grey;
}
```

Remember our parents and children from our HTML. This is what we are targeting in our CSS here, all the children with the class `lede` that are inside the parent with class `feature`

Now we've seen _how_ we write CSS, let's take a look at how we include it within our HTML so our webpage can see it.

