1. Intro - Why should you care/ do this
2. Example of what we're building
3. Basic Overview of Codepen (a few sentences). Create an account in code pen.
4. The entire coding session should take place in codepen
5. Make user create 1 element, explain what happened (this work well for the jQuery guide)
	1. Description of HTML elements
	2. CSS selectors, etc.
	3. Assets (pictures, etc.)
	4. Encourage users to make changes
	5. add your own assets
	6. update headers, picture, css styles
6. How to share with your lover
7. Users can share full-screen links if they have an account example
8. Next steps / stretch goals

<hr>

Valentine’s Day is just around the corner, and there's no better way to someone's heart than a handmade card - which is exactly what we're making in this tutorial. Using the power of HTML and CSS, you'll learn how to develop a website that doubles as a v-day card to wow that special someone in your life.

### HTML and CSS

Websites are made up of many things, but HTML (Hyper Text Markup Language) and CSS (Cascading Style Sheets) are the two main components. Together, they are the building blocks for every single webpage on the Internet.

Think of a greeting card. It's made up of many attributes, like text, an image, and perhaps a poem of sorts. In the world of HTML, such attributes are the elements of a webpage. Meanwhile, each of the card's attributes are usually different. Perhaps they differ by size. Or shape. Or color. Back in the web world, CSS is used to define the look and feel of a webpage. 

> Remember: HTML provides structure, while the CSS is used for styling, making websites look pretty. LINK TO HTML/CSS BASICS TUTORIAL

Now let's turn to an actual web page ...

IMAGE (http://cssdeck.com/labs/full/u3hephct)

The image above is an example of what we're going to be creating, with just HTML and CSS. 

### Setup

For this tutorial we will be using an online HTML, CSS, and Javascript code editor called [CSSDeck](http://cssdeck.com/). Sign up for a free plan [here](http://cssdeck.com/signup). After signing up, navigate to the homepage and click the "New" button to create a new environment for us to work in. 

You should see four panes. The three smaller panes on the left are for entering your HTML, CSS, and/or Javascript code, while the large pane displays a preview of the how the webpage will *actually* look.

### Our Card's Structure (HTML)

We'll be using the following HTML tags to develop our card-
- Header: `<h1>`
- Image: `<img>`
- Paragraph: `<p>`
- Divider: `<div>`
- Anchor: `<a>`

Each of the tags will be styled using CSS. We'll also be applying a border around the entire webpage, which is stictly a CSS style.

#### Add basic structure

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

Copy and paste this basic webpage structure into the HTML pane within CSSDeck. This structure is commonly referred to as a boilerplate template. These are used to speed up development so you don't have to code the features common to every single webpage each time you create a new page.

**What's going on?**

1. The first line, `<!DOCTYPE html>` is the document type declaration, which tells the browser the version of HTML the page is using (HTML5, in our case).
2. `<html>` informs the browser that all code between the opening and closing, `</html>`, tags is HTML.
3. The `<head>` tag contains links to CSS stylesheets and Javascript files that we wish to use in our web page, as well as meta information used by search engines.
4. All code that falls within the `<body>` tags are part of the main content of the page, which will appear in the browser to the end user.

This is how a standard HTML page is structured.

Add a the following element to the page within the `<body>` tags:

```html
<h1>Hello, World<h1>
```

Check out the preview pane. You should see the header you just added.

Congrats! You just made your first webpage.

[http://cssdeck.com/labs/kz8sc3zw](http://cssdeck.com/labs/kz8sc3zw)

#### Page title

Add a title to your card between in the page head (`<head></head>`): 

```html
<title>Happy Valentine's Day!</title>
```

#### Header

Update the header in your card:

```html
<h1>Happy Valentine's Day<h1>
```

[http://cssdeck.com/labs/62mmslgp](http://cssdeck.com/labs/62mmslgp)

Headers include the `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` and `<h6>` tags. `<h1>` is the main heading and the remaining headings decrease in size, with `<h6>` being the smallest. It's best practice to use the `<h1>` tag only once per page, while the other tags can be used any number of times, but they should always be in order. In other words, `<h3>` should be a sub-heading of `<h2>` and `<h4>` should be a sub-heading of `<h3>`, and so forth. 

#### Image

Insert an image just below the header:

```html
<img src="http://i.imgur.com/a2tjOcm.png">
```

[http://cssdeck.com/labs/ohqmko16](http://cssdeck.com/labs/ohqmko16)

#### Paragraph Text

Say something sweet. Add some paragraph text:

```html
<p>Write your personal message here</p>
```

[http://cssdeck.com/labs/ofag2kig](http://cssdeck.com/labs/ofag2kig)

#### Button

Let's create a button that links to a video:

```html
<div>click here to get your present<div>
```

Doesn't look much like a button yet. *Hint: That's where CSS comes into play.**

[http://cssdeck.com/labs/1opjhgbg](http://cssdeck.com/labs/1opjhgbg)

####

Finally, surround the button with a link:

```html
<a href="/"><div>click here to get your present<div></a>
```

[http://cssdeck.com/labs/m9d3pqjy](http://cssdeck.com/labs/m9d3pqjy)


### Our Card's Style (CSS)
