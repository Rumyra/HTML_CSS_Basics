# Form Submit

There is one more thing we must remember when writing the HTML for a form and that's a submit button, which the user presses to send the information they have entered.

There are two ways to do this, you can use either.

The first is the `input` element we have seen before:

`<input type="submit" />`

With a type `submit` we don't need a label here, as as you can see the browser has created a button for us. If we want to change the text in the button we can add that `value` attribute on the input:

`<input type="submit" value="New Text" />`

The other way is to use a `button` element.

`<button type="submit">Send Form</button>`

This creates the same functionality, when a user clicks it the form data will be sent. You only need _one_ per form and it can be either of these.

So there we have it! You have built your first form, well done this is a huge part of how the web is built. Now let's move on to the next chapter 
