# CSS Grid

Let's take a look at CSS Grid, out third way of laying things out with CSS.

You may have heard that CSS Grid is new, but it's been around for over two years! In web that's not actually that new. It's very well supported (that means you can use it and it will work in all modern browsers) and it makes our blog page layout very very easy.

Just liek the flexbox video, this is an introduction, as there's lots and lots to CSS Grid. We made a whole in depth course on it! So make sure you check that out once you've finished this course, do you can become a grid master.

To use CSS Grid it's a lot like Flexbox, you have to set the display property on the parent element:

```css
section {
	display: grid;
}
```

This means all the direct children of that element will be affected by CSS Grid. But we also have to define the grid we want. We do this by setting columns and rows, which create cells (a bit like a table), and we can place our elements within those cells.

We set how many rows and how many columns we want on the parent element. We do this by saying how big we want them, and how many mesurements we use tells the grid how many rows or columns there are overall. Let's look at an example:


