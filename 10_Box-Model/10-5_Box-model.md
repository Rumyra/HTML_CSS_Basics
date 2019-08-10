# Box Model

One really important concept we should dicuss about CSS layout is what we call the box model. It's all about the way the elements box works in relation to it's display type, the margin, padding and border that is applied and any sizing, like width and height. Basically all the things we have covered in the chapter so far.

Once we've got an overview of this, we can go on to move our elements around and get them in the right place.

Let's take a look at one of our elements with devtools again.

...

```css
p {
	width: 50%;
	margin: 20px;
	padding: 20px;
	border: 10px solid red;
}
```

We can see the blue area this paragraph takes up.

In devtools you can see this, to teh bottom right of the styles panel there's an orange box. It shows the area the content takes up in the middle - this is called the _content box_. When we set the width and height of an element, it's this box we are setting it on. There's a css property which dictates it called `box-sizing` and by default it's set to `content-box`

```css
p {
	width: 50%;
	margin: 20px;
	padding: 20px;
	border: 10px solid red;
	box-sixing: content-box;
}
```

Only then do we have the padding and the border. So the actual size of the element when it's displayed on the page takes up the width _plus_ the padding _plus_ the border.

So if we think about the width of the paragrpah, we have 50% plus on side of padding which is 20px, plus the other side - another 20px, plus both border sides - two times 10px - our actual width id 50% + 20px + 20px + 10px + 10px which is 50% + 60px! This could cause problems if we want to put two paragrpahs next to each other as we might assume them being both 50%, taking up half the width, they would fit. Not with the extra width added here.

The content, padding and border make up a box called the border box.

If we change our `box-sizing` property to a value of `border-box` we'll see our paragraph get smaller. Now the width we have said takes into account this border box, so the padding and the border as well as our content. THis is great because it meane we don't have to worry about all that maths!

Then there's the margin as well. This isn't part of the content of the element, as it doesn't sit inside, it sits outside, so we can't control it, we must remember it is there.

One thing to note about margins is margin collapsing. If two margins are sitting next to each other, from two elements that are next to eac other (top and bottom, or left and right), the biggest of the two margins will make the gap, rather than both. Let's take a look.

Both of these paragraphs have a margin of 20px, but if we inspect them you can see the entire gap is just 20px, not 40 - that's because they have _collapsed_.

Remebering all these things about an element and the box model and also the difference we saw between block, inline and inline-block elements before, we give us a really good grounding for when we come to laying out our page in the next chapter.