# HTML Syntax

Let's dive right in and take a look at how we write HTML. All HTML Elements follow the same format. You write the name of the element inside square brackets, then you can write the content after, then you do what we call _close_ the element, by writing the same element inside square brackets again, but with a forward slash after the first square bracket.

Write a p and img - then exercise can start next chapter with page structure.

Let's take a look at a paragraph element. This is used to tell the browser a block of text is there.

We open our angle bracket, use the correct element, for a paragraph it's a p, we add a closing angle bracket. Now we have written our element, we can add our content. For a paragraph it's more than likely words. But what we have to do after that is _close_ our element ready for the next one. To do that we open our angle bracket again, this time put a forward slash, write the element, our p and then close our angle bracket.

`<p>Hello Ultimate Courses!</p>`

Let's take a look at another example, this time heading text. We talk through different elements as we go through the course, so for this example let's use a top level heading, we describe this as an h1.

We open our angle bracket, type h1 which is our element, type our closing angle bracket. Write our header, then close our element by writing it again but this time with a forward slash.

`<h1>Our Cool Site</h1>`

Now let's take a look at a different style of element. An img element. We'll introduce a couple of extra things whilst we do this. An img element is slightly different as it doesn't contain any content we create ourselves, what we want to do is set a reference to an image file that is shown on our webpage.

We can do this with what we call attributes. These are extra bits of information we add to the element, which tells the browser more about the element itself. These attributes are either be defined or in some special cases we can choose what they are as long as we follow a certain set of guidelines.

So for an image element we open our angle bracket and write the element we want to use, in this case img but instead of writing a closing angular bracket straight away we want to tell this element where to find the image file. We can do this via the src attribute.

Attributes are keywords that are writen within the angular brackets when defining the element. You write what the attribute is, then you write an equals sign, then open double quotes (you can use single quotes here, but it's standard to use double quotes so we'll stick with the standard) then we put in the value for that attribute. In this case it's the file name of the image.

We then close the quotes. Our attribute is written!

There are a few types of attributes to mention at this stage. There are required attributes, which mean the element you are writing needs them, this is the case with the src attribute of the image element. We always need to tell the browser where the image is, so we always need to write it. There are optional attributes, these are used to modify the default behaviour of elements. And there are also standard attributes which are supported by the majority of elements. We'll look at these as we work through the course.

Back to our image element though. There is another required attribute for this element, it's the alt attribute. The value it takes is a description of the image. It's used if the image doesn't load, or by assistive technology to describe to the user what the image is if it can't be seen for whatever reason.

Let's add that to our image element.

`<img src="" alt="" />`

There is one last thing about our image element. It doesn't close the same way as our previous two examples, it's a self closing element. Because we reference the content by linking to an image file, we don't need to add any in ourselves, so we can just type a forward slash and then the closing angle bracket. There's a couple of elements that work like this and when we come across them we will note them.

Before we finish talking about the basic syntax of HTML, let's look at how we write comments. Comments are used in code to write things that the program looks over when running. It means we can easily annotate our code for ourselves and other developers.

In HTML you write a comment by using angular brackets again, but this time you use an exclamation mark and two hyphens, this is recognised as a comment and you can write whatever you want now. Once you're done you type two hyphens and the closing angle bracket to close it out. Your code editor should highlight the comment differently so it's easy to recognise.

<!-- this is an HTML comment -->

Whitespace

Now that we've covered the basic syntax, let's move on by creating our first webpage file.