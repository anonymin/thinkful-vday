---------------------------------


#### Border

```CSS
body {
  border: 20px solid #fcd2d8;  
}
```
The border property contains the following values - 
`border-width` `border-style` `border-color`

Try changing these values. Play with the pixel size until you get the right width. Try a `dashed` or `dotted` value for the style, and find a pretty color [here](http://color.hailpixel.com/). *Developer hint:* Use that special someone's favorite color!

#### Header


update to paragraph ...

Add the following header to your card beneath the opening `<body>` tag:

```html
<h1>Happy Valentine's Day<h1>
```

Headers include the `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` and `<h6>` tags. `<h1>` is the main heading and the remaining headings decrease in size, with `<h6>` being the smallest. It's best practice to use the `<h1>` tag only once per page, while the other tags can be used any number of times, but they should always be in order. In other words, `<h3>` should be a sub-heading of `<h2>` and `<h4>` should be a sub-heading of `<h3>`, and so forth. 

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

EXPLANATION

#### Image



#### Paragraph Text

#### Button

### Sharing

Show that you care.

### Next Steps

### Conclusion







Let's look at a quick example before building our card. 

#### HTML

The following HTML code displays the text, "Hello, World".

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Bootstrap 101 Template</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="http://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap.min.css" rel="stylesheet" media="screen">
  </head>
  <body>
    <div class="container">
      <h1>Hello, world</h1>
    </div>
  </body>
</html>
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
