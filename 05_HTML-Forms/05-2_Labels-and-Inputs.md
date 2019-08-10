# Labels and Inputs

If we take a look at a form, we would more than not see a box that as a user we could type text into. This is called an input.

Along with that box we have text, hopefully sitting somewhere above or beside it, saying _what_ to type in to that box. This is called a label.

When we put HTML in the form we created in the previous video, we add these two elements together. A label element and an input element.

Let's start with the `label` element.

`<label>Username</label>`

The label element needs an attribute to tell the browser which input it is for. That's the `for` attribute. We can write whatever value we want in the `for` attribute.

`<label for="username">Username</label>`

The input element is another special element like image, which doesn't have any content inside it. The browser creates a box for us, so we make it self closing:

`<input type="text" />`

See how the browser has created a box for us. We have to specifiy a `type` attribute for an input element, as there are lots of different inputs you can have in a form, which we'll look at in a bit. This one is a `text` type, because we enter text into the box.

Remember how we had a `for` attribute for the label, well we need a matching attribute for the input, so they can find each other. This is the `id` attribute, it has to have the same value as the for. In this case _username_.

`<input type="text" id="username" />`

There is one more attribute inputs usually have, and that's the name attribute. When you send the data of the form away, what ever the user writes in the text box is sent, but we need to send something to identify what that is. This is what the name attribute is for. Again it can be whatever you want.

`<input type="text" id="username" name="user" />`

Now we understand the basics, let's move on and look at the different inputs you can have in a form.