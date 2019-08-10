# Colour Values

There's lots of properties in CSS that need a colour value. We've already seen `border-color`, but there's backgrounds and fonts and other things we'll cover. So it's a good idea at this point to go over what we can use _as_ a colour.

There's colour names. These are a list of predefined colours we write as just the name of the colour. You can find a full list in the resources, but it's things such as `red`, `blue` or `black`.

Note there's also a `transparent` keyword.

So you would use it thus:

```css
p {
	border-color: red;
}
```

This is easy and good in these videos to use as examples as writing `red` obviously means the border is going to be red. But these colours are pre-determined. That means if we have a design for a web site or a web app, which we more than often do, the colours in that design most likely won't match the colours we have as these words.

There are other ways we can write colours to make sure we can match correctly however.

Hex codes are a common format for colour. These are a 6 digit code with a hash symbol at the beginning.

```css
p {
	border-color: #ff0000;
}
```

As well as hex codes, you can write the colour with an rgb function. Remember our url function for loading files, it's just like that, but instead of putting url we put rgb and brackets.

```css
p {
	border-color: rgb(255, 0, 0);
}
```

Inside those brackets there are three comma seperated values. They are all numbers ranging from 0-255, the first one is red, the second is green and the third is blue. Each number says how much of these colours is mixed for the final colour. Again you would most likely use a tool to find out what the values were for the colour you were using.

There's an anotehr function just like rgb, which is rgba. It's the same as what we've jsut seen, but involves one extra value, a number between 0-1 for the alpha channel of a colour. This means we can set see through colours.

```css
p {
	border-color: rgba(255, 0, 0, 0.5);
}
```

See the function has changed to `rgba` and we've added a `0.5` after the red, green and blue values. Now the red colour is see through.

There's another similar function to rgb, it's called hsl. It represents hue, saturation and lightness. It's very similar in the fact we call it as a function. But the values are different.

```css
p {
	border-color: hsl(200, 50%, 50%);
}
```

The hue is a value between 0-360, which is the colour wheel goin round in a circle. R O Y G B P - R = 0 , P = 300. The saturation is how bright the colour is, so none would be grey and full would be very flourescent. Notice how this is a percentage, so take sa value between 0-100, and you need a percentage sign.

The same is true for lightness, but this represents how light the colour is. Just like rgb, the hsl function has an alternative hsla, which has an alpha channel.

```css
p {
	border-color: hsla(200, 50%, 50%, 0.8);
}
```

The benefit of hsl is once you get used to where the colours are on the hue values, it can be more human readable than egb, as mixing red, green and blue is difficult.

You might wonder how you find the right code for a design, like a hex code, or rgb values. Mac computers have a colour tool built in, so you can use that to _pick_ the colour from the design. There's this ...


