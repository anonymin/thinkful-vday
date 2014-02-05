


#### Border

```CSS
body {
  border: 20px solid #fcd2d8;  
}
```
The border property contains the following values - 
`border-width` `border-style` `border-color`

Try changing these values. Play with the pixel size until you get the right width. Try a `dashed` or `dotted` value for the style, and find a pretty color [here](http://color.hailpixel.com/). *Developer hint:* Use that special someone's favorite color!



Next, add a CSS selector to the opening `<h1>` tag:

```html
<h1 class="header">
```

With this tag, we can assign styles to it by referencing it in our CSS stylesheet:

```css
h1 {
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", sans-serif;
  font-size: 68px;
  text-align: center;
  margin-top: 50px;
}
```





#### CSS

The following is a what a standard CSS stylesheet looks like:

```css
.container {
  padding-top: 50px;
}

body {
  background-color: yellow;
}
```

**What's going on?**

1. The `.container` selector is associated with the same selector in our HTML document (check it out), followed by curly braces.
2. Inside the curly braces, we have a properties, which are descriptive words, like font-weight, font-size, or background color. In our case, we have `padding-top`.
3. Values are then assigned to each property, which are preceded by a colon and followed by a semi-colon. 

  > http://cssvalues.com/ is an excellent resource for finding the acceptable values given a CSS property. 

Can you figure out what's going on with the body tag?
