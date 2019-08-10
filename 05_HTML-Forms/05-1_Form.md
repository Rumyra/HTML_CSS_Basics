# Forms

Forms are really important when building websites and web apps. You probably don't notice them so much anymore because the user experience (or UX) of forms is pretty smooth in most cases these days.

But they are used every time we want to pass data from a webpage to either another webpage or a database.

Imagine when you log in to a site, that's a form, or update your status, you're filling out a form. If you built your own site and wanted to have a way for people to send you messages, that would be a form.

Everytime you search for soemthing via google - yup you got it, a form.

So let's take a look at how we build them.

The first element we need is a `form` element. This wraps all the other elements we're going to look at in this chapter:

`<form></form>`

Really big forms, like those which you fill out when applying for insurance, that needs lots of details, like your name, address, past details etc... have sections within them.

In a form they are called a `fieldset`

```html
<form>
	<fieldset>
		
	</fieldset>
</form>
```
Because you usually have more than one _fieldset_ within a form, each one has a heading. In forms they are called `legends`

```html
<form>
	<fieldset>
		<legend>Form section</legend>
	</fieldset>
</form>
```

You can see how this looks in our browser. It's drawn a line around the fiedset area and written the legend in the top.

Once we've got our form we can start putting what we call inputs inside it.