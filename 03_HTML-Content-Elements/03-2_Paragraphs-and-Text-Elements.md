# Paragraphs and Text Elements

As well as headings we need paragraphs of text within our page. These are described with a p element.

`<p></p>`

The p element is used for blocks of text, or sentences, even one words sometimes. Content can not stand on it's own, so any text you have is usually wrapped in a p tag.

`<p>This is a website</p>`

`<p>Put the text from the design in here</p>`

There are also a number of elements to describe text. Let's look at some of the common ones.

If text has inportance it is wrapped with a `strong` element.

`<p>There is some text here <strong>and this is important</strong></p>`

Note how the browser styles the strong text in bold. This is default styling by the browser which we can change with css later, so this element is not for styling, but for describing the content inside it. If you do want to just have bold styling, even though there is no change in the content, there is a bold tag, whcih we type with a b.

`<p>There is some text here <b>and this text is styled bold</b></p>`

This pattern is the same for italic or slanted text. To emphasise words there's an element, we write it with `em`:

`<p>There is some text here <em>and this is emphasised</em></p>`

The browser styles this with italic text by default, but the element should be used for emphasised text and if we need to change the loook of it we can do that with CSS which we will learn later. If we purely want italic text we can use the i element.

`<p>There is some text here <i>and this is italic text</i></p>`

Sometimes we may need to target text to change the style of it in any way we choose, without any suggested defaults, or suggested content. There's an element for that, it's called a span. It doesn't suggest any content to the document, nor cause the browser to add any styling.

`<p>There is some text here <span>and this is some more text</span></p>`

Another element to note is the `time` element. This is used if you need to denote a specifc period of time, like a duration or date.

`<time>25th December</time>`

Or

`<time>Ten o'clock</time>`

The `time` element take an optional, but specific attribute. The `datetime` attribute. The value is also very specific, it depicts the time within the element as a machine readable string of characters in a format so the program can read the time as well.

So for our examples we would have:

`<time datetime="12-25">25th December</time>`

Which is the month and day. Or...

`<time datetime="10:00">Ten o'clock</time>`

Which is the time. There's a whole list of all the formats you can use in the resources for this course.