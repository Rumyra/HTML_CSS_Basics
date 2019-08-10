# CSS Floats

There are lots and lots of ways to move things around a web page or app with CSS. We covered styling and how the elements work with boxes. This is a good place to start, but now we need to move them.

Floats is the oldest method and was neevr originally meant for layout. As with all original CSS, it has ties to documents. If you consider a word doc for instance, and you want to put a picture in amongst words, you might want to have the words surrond the picture.

IMAGE HERE

That's what floats were for. It's original intention was to allow content to flow around another element. Let's see this with an image and text.

ARTICLE PAGE MARKUP

```css
img {
	float: right;
}
```

You can see the paragraph has surrounded the image. You may not be able to tell here, but what has also happened is the image has come out of the flow of the document, let's make the paragraph smaller and you will see.

The content below it can not _see_ the image, and so moves up underneath it, just like it would normally under the paragraph. This can case somewhat erratic behaviour when working with floats as a layout method rather than just moving content around something.

Before we take a look at another example and the fix for this, let's just revise the values we can use for the float property.

We used `float: right;` which moved the image to the right. By default elements are not floated and their value is `none`, you can also float the `left`. There's a couple of other values, but let's stick with these for now.

So let's use floats to get our sidebar to the right of the main area:

PUT IN CORRECT CSS

```css
main {
	float: left;
}

aside {
	float: right;
}
```

As you can see, although these elements are on the left and right, there isn't enough _room_ for the sidebar yet, even though the widths add up to 100%. This is because we have padding on them. Remember how padding is added to the width. Let's change the box-sizing to border box:

Now the floated elements have enough room to be next to each other. But we have another problem. Because both elements have jumped out of the normal flow of the document, the footer has jumped up to where the header is. This content isn't being seen by the rest of it anymore.

There is a fix for this. What we need to do is give tell the containing element the contents should be in normal flow again. We can do this with a couple of different css properties. We onlt need one.

The legacy way we've done this is to add `overflow: auto` to the parent element. This tells the parent element that yes the floated elements are inside.

...

There are a couple of problems with this however as this property was never meant for this purposes. The overflow property is used to say how we want the box to behave if content goes outside the bounds of the element, for instance `hidden` is a value and that would mean crop the content, or `scroll` which would let the parent display scorll bars. So on a few occasions you might experience some erratic behaviour. However it is very well supported.

Instead of `overflow: hidden;` There is a new property `display: flow-root;` which does teh same thing, it tells the parent element there is content inside and allows it to be the size it _should_ be. However some old browsers, like internet explorer do not support this. But for the purposes of our examples using it is fine, so let's do that instead.

Now the footer is at the bottom of the page again, we;ve manged to move the boxes left and right.

Something to note is, we could have actually floated both of them left, rather than one left and one right. This is because the sidebar would float up to the left side on the main section, so either would be allowed here.

The nav has all the links next to each other. Let's see what happens if we use floats to position all of them next to each other.

Let's float all the `li` elements right.

...

You might think this seems like a good idea, but look closer at the order of the links, they are now backwards. This is because the first 'home' link has floated right first, then the '' next and so on. So maybe this isn't the right method for the links.

One thing about CSS layout methods is there are quite a few of them, and it's just experience from practise which allows us to choose the best one.

Do you remember our display types. We could just harness them, if we give the `li` elements a display type of `inline-block`, they will be displayed inline, so all next to each other, but also act as boxes, so when we add margin and padding they will work nicely.

However, when we come to put the gap inbetween them things can get a little fiddly, as we have to just put a gap on the left of each one, as we want them flush on the right side. It would be nice if we could evenly space them within the nav itself.

There is a way to do this, it's the next layout method, so let's move on to take a look at it.