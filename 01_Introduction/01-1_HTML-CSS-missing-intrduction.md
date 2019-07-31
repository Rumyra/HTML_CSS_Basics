# HTML CSS Basics Introduction

>Slide: Intro

Welcome to the HTML and CSS Basics course with me Ruth John.

HTML and CSS are essential for creating any website or webapp and in this course we're going to start at the very beginning and work our way up to cover HTML and CSS to a professional level.

>Slide: Who This Course Is For

- Beginners wanting to learn HTML & CSS
- Intermediate developers who want to refresh their knowledge
- Senior developers who want a deeper understanding of the all the features HTML & CSS have to offer
- Teams looking to onboard and streamline development
- Learn fast but comprehensively
- Industry standard HTML & CSS knowledge

Whether you're a complete beginner, or a seasoned professional, this course has been designed to teach you up to date HTML & CSS coding practises and techniques. We'll start with an overview of what HTML and CSS are, where they came from and how we use them together. We'll cover the building blocks of both languages, which will in turn give us the capabilities of coding our own website project, with ease, using the knowledge we have learnt. I'm here to help you over come any nuonses we may come across as we build our way through the course.

>Slide: HTML

Let's start with HTML. HTML stands for HyperText Markup Language. The HyperText part describes the web itself - how text is _hyper_ linked and thus websites (which are built with HTML), if available on the internet, are accessible from a browser on the very computer you're working on at the moment.

The part that really describes what HTML is is the _markup language_ part. A markup language is one which _marks up_ content. HTML is a descriptive markup language. In our case, it describes the content parts of a website like words, images, videos and and such. The parts that described this content are called elements, or tags.

>Slide: Structure

In this course we'll cover the specific way of writing these: Our HTML syntax. We'll cover lots of different elements you can write which come together to form a website. You'll discover the best practises for coding each of them as we work our way through.

DO YOU WANT TO TALK ABOUT INTERPRETED LANGUAGES & THE BROWSER INTERPRETING HTML?

>Slide: History

Sir Tim Berners-Lee first proposed an internet based hypertext system in 1989. An initial version was avaliable in 1991 comprising of 18 elements.

Since then HTML has become the standard for describing website content and there are over 100 elements.

>Slide: CSS

HTML just describes the content we show on a screen when we display a website, it does not describe how that content should look.

Programmes that run HTML, like the familiar browser, apply default styling to each element to make HTML documents readable. But as developers we can use CSS to modify and override that styling, making it look unique and exciting.

CSS stands for Cascading Style Sheets. It was specifically designed for styling HTML on the world wide web and the first version (CSS1) was released in 1996.

In this course we'll cover the Cascade part of Cascading Style Sheets in detail. For now let's discuss the Style part. CSS declares styles for specific HTML elements in a number of ways. This can be how big the element is, what colour it is and where it is positioned within the browser when we view it.

We can write these styles in a seperate file, which allows us to have common styles for more than one HTML page we write. We'll look at different places we can write CSS within the course, how they affect the HTML differently and the benefits.

I'M GOING TO COME BACK TO THIS WITH NOTES FROM THE CURRICULUM

W3C
Browser support

HTML will run no matter what. Which means you won't get any nasty errors, but it also means you have to be very careful of what you type. The browser will try to close elements automatically. If you have a number of unclosed elements this can cause confusion and the affect CSS can get confused.

It will also parse elements which don't exist, so you can very easily mis type or mis spell HTML elements and the browser won't mind. Again this can cause problems, as the browser interprets the content it sees and won't be able to do so if it doesn't recognise the content.

You can check you HTML by going here and copying and pasting the code in, it will show you any errors that reside in it.

CSS is different. It won't run if you write it incorrectly. The browser is still pretty forgiving and will try and run it, however you can check CSS easily by opening devtools.

To see HTML and CSS in devtools, you inspect and element. Here in the devtools panel you can both the HTML elements and the CSS styles. If we incorrectly type a CSS style, Chrome will display a warning icon next to the style and cross the style out.

Note that this is different to a style being over ridden, which happen a lot with CSS, whereby the style will just be crossed out. If you're having trouble, inspect your element and check your CSS, if you have a warning icon it means your CSS is incorrect.


It also allows us to have different styles for different environments. Consider if you wanted to print a webpage, you may want to adjust the styles you have applied to your HTML elements to optimise for printing, such as black text on a white background for example. 

HTML files are held on the server. The first file a server looks for by default is usually called `index.html`, but you can call it whatever you like. It's good practise however to not put spaces in the names of your files, as computers have to convert spaces to symbols and this can cause erratic behaviour on different systems. So as developers we usually use underscores _ or hyphens - in file names. 

HTML is written following a data structure, based on another language called XML.

Child parents

Accessibility https://hacks.mozilla.org/2019/06/how-accessibility-trees-inform-assistive-tech/