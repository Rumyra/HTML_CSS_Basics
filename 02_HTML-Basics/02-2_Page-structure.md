# Page structure

Now we know how to write HTML elements, let's take a look at how an HTML document is structured.

If you open index.html from the project files we can do this together.

Every HTML file needs a doctype declaration at the top to tell the program that is reading it that it is in fact an html file.

`<!DOCTYPE html>`

This doesn't need a closing element, it is mearly a declaration stating it's a document of type html.

Once we've got that everything within the page we're about to write needs to be held in html tags, so let's put those in. A good technique when writing html elements is to open and close them at the same time, so you don't forget to close them.

Let's create out html tag and close it. Open our angle bracket, write html, close it and open our closing tag, don't forget our forward slash, then write html and close our angle bracket.

`<html></html>`

Now we need content _inside_ this element, so put your cursor back to the middle of this element. Press enter or return a couple of times and we're ready to put content in our page.

The html element takes a language attribute, you write it like this:

`<html lang="en">`

The attribute is lang and the value here is en, which stands for english. There are set abbreviations for all languages, so the browser and assistive technologies know what language to expect the content to be in.

There are two child elements of the html element, the head and the body. Let's start with the head element.

Remember our spacing, because it's a child we want to tab in once.

`<head></head>`

We'll take a look at the content of the head element in detail in the next video, but for now let's add our body element in as well.

One thing to note here is most text editors have an auto complete function, which means when you start typing an element, you can press tab or enter and the whole element will be completed for you.

`<body></body>`

There two sections are very important as they structure our whole html page. All the content the user sees on the page is held within the body element. The head element contains more information about the page for the program that is reading it.

In the next video we'll look at what we need to add inside the head element.
