# Falling in love with HTML and CSS

Please note: This is a presentation/training mean to be paired with this [blog](http://www.thinkful.com/learn/valentines-day-ecard) post. 

## Basic TOC

1. Intro
2. Example of what we're building
3. Requirements
4. Code Workflow
  - HTML elements
  - CSS styles
6. Next steps
7. Your turn!

## Intro

Web developers use HTML (or Hypertext Markup Language) to tell web browsers whether the elements and text found on a web page is, well, HTML. Web browsers, in turn, use this information to structure and display the page as described in the actual HTML file. Meanwhile, CSS (or Cascading Style Sheets) is used to make web pages attractive/pretty. For example, developers use CSS rules to change the font color, font size, the typeface of text, and so forth. 

Let's start with the structure, but first let's look at what we're going to be creating today:

![final](https://raw.github.com/mjhea0/thinkful-vday/master/images/final_card.png)

You can also view the final webpage [here](http://cssdeck.com/labs/full/npulm7vr).

## Requirements

Before we start, you need a *source code editor*, which is simply a text editor designed specifically for writing source code. Some popular editors include Notepad++ (Windows), TextMate (Mac), and Gedit (cross-platform). For this exercise, please download the cross-platform editor [Sublime Text](http://www.sublimetext.com/2), which is an editor designed for simplicity and ease of use.

Also, please make sure you have [Google Chrome](http://google.com/chrome) installed.

**Break out Sublime (or our favorite editor). Let's code.**

## Workflow

We will be creating this was page iteratively, step by step. In other words, we'll add a line of code then discuss what it does.

## Our Card's Structure (HTML)

We'll be using the following HTML [tags](http://www.htmldog.com/guides/html/beginner/tags/) to develop our card:
- Title: `<title>`
- Heading: `<h1>`
- Image: `<img>`
- Paragraph: `<p>`
- Divider: `<div>`
- Anchor: `<a>`

Many of these tags will be styled using CSS. We'll also fancy it up by applying a border around the entire webpage, which is strictly a CSS style.

### Add basic structure

```html
<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <body>
  </body>
</html>
```

Copy and paste this basic webpage structure into your text editor. Save this file as *index.html*.

This structure is commonly referred to as a boilerplate template. Such templates are used to speed up development so you don't have to code the features common to every single webpage each time you create a new page. Most boilerplates include much more features, but let's start with the basics.

**What's going on?**

1. The first line, `<!DOCTYPE html>` is the document type declaration, which tells the browser the version of HTML the page is using (HTML5, in our case). 
2. `<html>` informs the browser that all code between the opening and closing, `</html>`, tags is HTML.
3. The `<head>` tag contains links to CSS stylesheets and Javascript files that we wish to use in our web page, as well as meta information used by search engines.
4. All code that falls within the `<body>` tags are part of the main content of the page, which will appear in the browser to the end user.

This is how a standard HTML page is structured.

Add a the following element to the page within the `<body>` tags:

```html
<h1>Hello, World</h1>
```

Check it out in Chrome. You should see the header text, "Hello, World".

Congrats! You just made a webpage. (Your first?!)

[http://cssdeck.com/labs/kz8sc3zw](http://cssdeck.com/labs/kz8sc3zw)

**What's going on?**

1. *Tags* form the structure of your page. They surround and apply *meaning* to content. There usually is an opening tag and then a closing tag, like - `<div></div>`, a divider. Some tags, like the `<img>` (image) and `<br>` (line break) tags do not require a closing tag. Notice how I included one `<br>` tag with a `/` on the end. This was a best practice in previous versions of HTML. HTML5, on the other hand - the version we are using - is much more relaxed and does not require a `/`, but it will work fine with it as well. It's really the developer's preference.
2. *Elements* represent the tags as well as whatever falls between the opening and closing tags, like - `<title>My bumblebee website</title>`

### Title

Add a [title](http://www.htmldog.com/guides/html/beginner/titles/) to your card between the opening and closing `<head>` tags: 

```html
<title>Happy Valentine's Day!</title>
```

### Heading

Update the [heading](http://www.htmldog.com/guides/html/beginner/headings/) in your card:

```html
<h1>Happy Valentine's Day</h1>
```

Headers include the `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` and `<h6>` tags. `<h1>` is the main heading and the remaining headings decrease in size, with `<h6>` being the smallest. It's best practice to use the `<h1>` tag only once per page, while the other tags can be used any number of times, but they should always be in order. In other words, `<h3>` should be a sub-heading of `<h2>` and `<h4>` should be a sub-heading of `<h3>`, and so forth. 

> Want it to say something different? Just change the text between the tags!

[http://cssdeck.com/labs/62mmslgp](http://cssdeck.com/labs/62mmslgp)

### Image

Insert an image just below the main heading:

```html
<img src="http://i.imgur.com/a2tjOcm.png">
```

[http://cssdeck.com/labs/ohqmko16](http://cssdeck.com/labs/ohqmko16)

### Paragraph Text

Say something sweet. Write your personal message within the paragraph text:

```html
<p>Write your personal message here</p>
```
> Tip: Replace "Write your personal message here" with your actual message. :) 

[http://cssdeck.com/labs/ofag2kig](http://cssdeck.com/labs/ofag2kig)

### Divider

Let's create a button using the divider tag:

```html
<div>click here to get your present</div>
```

Doesn't look much like a button yet. It will soon. Trust me.

[http://cssdeck.com/labs/1opjhgbg](http://cssdeck.com/labs/1opjhgbg)

### Anchor

Finally, surround the divider tags with an `<a>` tag to create a link:

```html
<a href="/"><div>click here to get your present</div></a>
```

You also need to insert a link to replace the slash in the `<a>`. You could add a link to a cute video from Youtube. To really wow your partner with your DIY gift, create your own video to link to! <3

[http://cssdeck.com/labs/m9d3pqjy](http://cssdeck.com/labs/m9d3pqjy)

Well, we've added all the HTML structure to our page:

![after_html](https://raw.github.com/mjhea0/thinkful-vday/master/images/after_html.png)

Check out the fullscreen preview [here](http://cssdeck.com/labs/full/m9d3pqjy).

Kind of bland, to put it nicely. Fortunately, we can quickly change that with CSS!

## Our Card's Style (CSS)

While HTML provides, structure, CSS is used for styling, making webpages look nice. From the size of the text to the background colors to the positioning of HTML elements, CSS gives you control over almost every visual aspect of a page.

CSS and HTML work in tandem. CSS styles (or rules) are applied directly to HTML elements using [selectors](http://www.htmldog.com/guides/css/beginner/selectors/). Simply add selectors (either IDs or Classes) to your HTML, and then you can link directly to them in your stylesheet.

We're going to add three selectors to our HTML page:

1. `.header`
2. `.msg`
3. `.button`

Insert them now:

```html
<h1 id="header">Happy Valentine's Day!</h1>
<p id="msg">Write your personal message here.</p>
<div id="button">Click here to get your present.</button>
```

Your code should now look like [this](http://cssdeck.com/labs/epx8vf9o).

Next, we need to "link" our HTML page and CSS stylesheet. To do so, add the following code to the `<head>` section of the HTML page just below the title:

```html
<link rel="stylesheet" href="styles.css">
```

### Header

```css
#header {
  font-size: 68px;
  margin-top: 50px;
  font-weight: normal;
}
```

Copy and paste this into the CSS a new file. Save it as *styles.css*. 

Here, we are increasing the size of the font, changing the thickness of the text, and adding some space to the top of our header selector. Try updating the size of the text. Or color. Play around with this.

**What's going on?**

1. We have the `#header` selector, which is associated with the selector in our HTML document, followed by curly braces.
2. Inside the curly braces, we have properties, which are descriptive words, like font-weight, font-size, or background color. In our case, we have `font-size` and `margin-top`.
3. Values are then assigned to each property, which are preceded by a colon and followed by a semi-colon. 

> Tip: http://cssvalues.com/ is an excellent resource for finding the applicable values given a CSS property.

[http://cssdeck.com/labs/ej1kciif](http://cssdeck.com/labs/ej1kciif)

### Paragraph Text

Update the style of your personal message:

```css
#msg {
  font-style: italic;
  font-size: 36px;
  color: #f12469;
  margin-top: 50px;
}
```

This changes the color of our text, italicizes it, changes the size. It also adds a margin to the top of the message.

[http://cssdeck.com/labs/brkeecsj](http://cssdeck.com/labs/brkeecsj)

### Divider

Let's make that button look like a button:

```css
#button {
  border-radius: 30px;
  height: 40px;
  width: 335px; 
  background-color: #f12469;
  font-size: 20px;
  color: #ffffff;
  margin:0 auto;
  padding-top: 15px;
  margin-bottom: 50px;
}
```

With this, our button becomes rounded. We set its height and width, and applied color changes.

> Have some fun with this. Change the `background-color` and well as the font `color`.

[http://cssdeck.com/labs/zh2itiuj](http://cssdeck.com/labs/zh2itiuj)

The text is still a bit off. Let's fix that.

### Additional CSS

```css
body {
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", sans-serif;
  border-width: 20px; 
  border-style: solid; 
  border-color: #fcd2d8;
  text-align: center;
}

a {
  color: #ffffff;
  text-decoration: none;
}
```

Try changing the border values. Play with the pixel size until you get it the right width. Try a `dashed` or `dotted` value for the style, and find a pretty color [here](http://color.hailpixel.com/). 

> Pro Tip: Use that special someone's favorite color! (You should know this ... if not, find out quickly.)

Check it out!

![final](https://raw.github.com/mjhea0/thinkful-vday/master/images/final_card.png)

[http://cssdeck.com/labs/npulm7vr](http://cssdeck.com/labs/npulm7vr)

## Your turn!

While I provide a brief review, work along with me while you develop your own basic site. Stick with the V-day theme for fun! 

1. Create a basic HTML page with the doctype, html, head, and body tags (remember the boilerplate template!)
2. Add a header (H1)
3. Add some paragraph text (perhaps a something special for your sweetie)
4. Add a link to this image: ![heart](),
5. Add an external CSS file (make sure to link to the HTML page)
6. Change the background color, then center all elements.

Sweet. Send me your code to review if you'd like to michael@mherman.org.

## Chrome Developer Tools

Using Chrome Developer Tools, we can test either HTML or CSS changes directly from the browser. This can save a lot time. Instead of firing up your text editor and getting your development environment setup. You can test out quick changes directly from Chrome.

Open up the HTML page we worked on. Right Click on the `<h1>` tag. Select "Inspect Element". Notice the styles on the right side of the Developer Tools pane associated with the paragraph. Do you see the styles associated with it. Try changng the size of the font as well as the color..

![dev_tools](https://raw.github.com/mjhea0/thinkful-vday/master/images/dev_tools.png)

You can also edit your HTML in real time. With Dev Tools open, right click the paragraph text and select "Edit as HTML". Add another paragraph.

> Be careful as these changes are temporary. Watch what happens when you refresh the page.

## Next Steps

- Did you customize the card? Try again. This time don't look at my code examples.
- Don't wait until the last minute. Get started on your St. Patrick's day card now!
- Add some JavaScript/jQuery. Check out my card [here](http://gleit.me)

## Conclusion

That's all I have planned. Thank you! Question time!

