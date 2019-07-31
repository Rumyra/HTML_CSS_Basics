# Head Information

Let's add content within our head tags. This content gives the browser more information about the webpage itself. Apart from a couple of small parts, when you view this webpage you do not see this information.

The first piece of information we'll add is the character set of the file itself. By default this is UTF-8. We do this with a meta element and a specific attribute.

`<meta charset="utf-8">`

The attribute here is the `charset` attribute. Where the value is utf-8. Elements in the head are special in that if they don't contain any content within them, like this example, they don't need a closing element. So we can just write this meta tag like this.

Another meta element we always add to the head to give the browser information is the viewport meta element. Your website of app will be viewed on many different devices, some of which have what we call retina screens. This means they have more pixels per area than other screens, more dots that display our website. It's preferable to normalise this for all devices so what we build is displayed at a standard size, otherwise on a retina screen (like an iPhone for example) our website can appear very small and zoomed out.

This element tells the browser to normalise this size and make one pixel appear the same across all devices, regardless of each individual pixel _density_.

`<meta name="viewport" content="width=device-width, initial-scale=1">`

Out last meta tag we're going to include is the description. It's written the same as the previous ones, however we have a desc attribute.

The description is important. Not only do search engines like Google read this information to see what this html page is about, they also display this information in the search results.

`<meta name="description" content="">`

All we have to remember with the content within this atribute is it needs to be unique. So copying content directly from the webpage itself will not suffice. Search engines are very good at picking up on that and lowering search result status because of it. Just describe your web page within the attribute.

`content="This is the portfolio website of Jo Bloggs, an illustrator and designer. View their work and contact them here."`

Now we can look at some content the user does see.

If you look to the top of your browser, or the tab you are using, you might see the title of the page. We show this inside the head element with the title tag. This is a content element, so it needs opening and closing.

`<title>My Website</title>`

Inside it you write your website or app title. It's good practise to put what page you are on as well, usually before the name of the site, that way if someone has two tabs with your website open they can see the page first:

`<title>Homepage | My Website</title>`

Every website or app also has an icon. You might see it when you look up at the tab when a webpage is open. Different platforms have different standards for these icons. The website standard is what we call a favicon. This needs to be in a file format of `.ico` if you look in your project files there is one there already for you. Because this icon is in the directory of the website, a browser uses it automatically for it's icon, so we don't have to do anything. An iPhone however will need a png format, so let's include that.

`<link rel="apple-touch-icon" href="icon.png">`

Here we are using the `<link>` element and two attributes. the `rel` attribute which discribes the relationship between the current document and the file. So in this case we are telling the document the file is a _apple touch icon_ for use on apple devices. we also need a `href` attribute which stands for hyperlink reference. The value of this attribute is the file itself. Here we also need to specify the file _extension_, or type, which you can see as the `.png` part of the file. You can't forget this.

There are lots of different icons for different platforms and devices In the resources you can find a link to generating these for you and the code to go along side it.

This `link` element is important and we'll be coming back to it later in the CSS part of this course. But for now, let's move on to the next chapter and start looking at content HTML elements for our web page.

