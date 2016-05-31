# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>

</body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
The first tag is self closing and the second tag is not.
```

---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Inline styles should usually not be used. They are applied to the tags themselves
in the html document.
Internal stylesheets are located in the html document, usually at the top. They
are not as preferred as external style sheets.
External stylesheets are styles located in a different file. This is preferable. 
All of these methods change styles and how the elements look on the page.
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* This will make a square block element more rounded on the edges */
div {
  border-radius: 50%;
}

/* Increases font size of the text in the paragraph element, which is in the 
header (or an element that has the .header class) */
.header p {
  font-size: 18px;
}

/* The element with this class (likely the footer) is 0 pixels from the bottom 
of its container element. It is absolutely positioned, which means it will not 
change when the window is resized? */
.footer {
  position: absolute;
  bottom: 0;
}

/* The element that has this class will display an image that completely covers
the area of its parent element. */
.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/* When you hover over the element with the .ninja class, the element will not 
show up and the color of the text will be black. */
.ninja:hover {
  display: none;
  color: black;
}
```

