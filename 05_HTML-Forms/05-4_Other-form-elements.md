# Other Form Elements

There are a few things you find in a form that are not written in the style of the `input` element, as we have previously seen.

The first you have probably come across and is referred to as a drop down.

This is written as a `select` element, with `option` elements inside it, that appear as the drop down options:

```html
<label for="selection">Choose an option</label>
<select id="selection">
	<option value="one">Option one</option>
	<option value="two">Option two</option>
	<option value="three">Option three</option>
</select>
```

Notice how we still use the `label` as before, with a `for` attribute and an `id` on the select element to link them together.

The `option` elements within the `select` have a `value` attribute. All inputs in forms can have a `value` attrribute. This represents what is input. For instance when we type text into a text box the value becomes whatever we type in. Because with the dropdown there's no way of inputting a value, we can define one ourselves. As I said we can use this attribute on any input.

As well as dropdowns, there are bigger areas of text other than just a small box. These are called textareas and are created using a `textarea` element. They are slightly different to inputs in that they need a closing element.

```html
<label for="message">Message</label>
<textarea id="message" name="a-message"></textarea>
```

We would use a text area in a situation where you would want a user to add more than just a couple of words of text, like a message or an article maybe.