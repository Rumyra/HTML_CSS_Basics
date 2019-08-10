# Different Inputs

The input type we already used was `text`, there's lots of types you can have. You can't make them up, they are set, but there are a lot to choose from.

Instead of setting the type to `text` we could set it to `password`, this would allow the browser to automatically hide the text that was typed in by the user.

```html
<label for="pass">Password</label>
<input type="password" id="pass" name="password" />
```

Notice how our `for` attribute on the label is the same as out `id` attribute on the input.

There's also an `email` type, which means the browser should pick up on an email format being entered into this box. Some browsers don't so be careful, you should use it as it's correct, but don't rely on it.

```html
<label for="email">Email</label>
<input type="email" id="email" name="email" />
```

There is also a `datetime` type, which allows a user to input a calendar style date. Most browsers show a date picker if this type is set, but again some don't so don't rely on it.

```html
<label for="date">Date</label>
<input type="datetime" id="date" name="date" />
```

You might want to allow the user to upload a file, for that there is a `file` type:

```html
<label for="file">Upload File</label>
<input type="file" id="file" name="file" />
```

If you want the user to have a box to tick, the type is `check`

```html
<label for="checkbox">Tick For Yes</label>
<input type="check" id="checkbox" name="yes" />
```

A very similar type to `check` is `radio`, the difference is radios are mutually exclusive. This means if you link them together in the code, only one can be selected at one time. Think of them like your multiple choice test, where you can only have one answer.

This means you need a group of labels and inputs, and they need to be all linked together.

Let's first write the labels and inputs:

```html
<label for="one">Choice One</label>
<input type="radio" id="one" />
<label for="two">Choice Two</label>
<input type="radio" id="two" />
<label for="three">Choice Three</label>
<input type="radio" id="three" />
```

Now let's group them together by giving all the inputs the same name attribute.

```html
<label for="one">Choice One</label>
<input type="radio" id="one" name="choices" />
<label for="two">Choice Two</label>
<input type="radio" id="two" name="choices" />
<label for="three">Choice Three</label>
<input type="radio" id="three" name="choices" />
```

There are a whole lot more, including types such as url, range and colour. You can find a link to a list of different ones in the resources of this course.

Let's move on to have a look at a couple of things you would find in a form that are not written as an `input`.