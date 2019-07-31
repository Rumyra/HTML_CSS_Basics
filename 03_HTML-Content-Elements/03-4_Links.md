# Links

A very important element on the web, are links, or rather as they are known _anchors_. Anchors link from one page to another page, or one site to another site, or from one part of a page to another part of a page.

They are written in a very specific way, as we need to tell the browser _where_ to link to. The anchor is the a tag:

`<a>This is a link</a>`

But the a tag needs an `href` attribute. This is short for hyperlink reference, which means a reference to where the link is going to go. It's inside this attribute we put the page or website we want the link to go to.

`<a href="https://ultimatecourses.com/">This is a link</a>`

If you are linking to another page on your website, you do not need to put the full url in, you can just put what we call a relative url in. This means a link _from_ where we are at the moment. So if we want to go from the index page to a contact page for instance and they are in the same place on our website, we would write something like this:

`<a href="contact.html">This is a link</a>`

