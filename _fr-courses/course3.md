---
layout: course-fr
title: Styling pages
number: 3
---

 Well now we know how to create a webpage and add link, but honestly, the result is ugly.
 First the links we have created previously are all on the same line, even if in the html page we set a carriage return after each link.
 Besides the text is black, links are with the old-fashion underlined blue style and the background is white.

 This is time to introduce css: cascade sthyle sheets.

Css is a separate file (or set of files) that will define the style to apply to the different elements (tags, class, id) of the page.
But why using a separate file? For many reasons but if you should only memorize 2 of them, these will be the following:
- defining styles independently of the page allows the reuse them for all the pages of the website, ensuring consistency in the website design and saving efforts of re-definition.
- when a website need a design refresh or let the user should the style he wants to apply, you just have to define another set of css files and the wole content will be restyled.

However css would be nothing without a few new tags to introduce:
- `<p>` defines a paragraph
- `<h1>`,  `<h1>`, ... defines different levels of title.

So now we are able to add style in our previous page:
```
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>add style!</title>
    <link rel="stylesheet" href="css/styles.css">
  </head>
  <body>
    <h1>We add styles!</h1>
    <p>Here is a list of links:<p>
    <p><a href="https://github.com/20centcroak/childrencourses">visit children courses</a></p>
    <p><a href="sample1.html">see sample1</a></p>
    <p><a href="https://github.com/20centcroak/childrencourses" target="_blank">visit children courses in a separate tag</a></p>
  </body>
</html>
```

and here is the styles.css content:
```
body {
  background-color: DarkTurquoise ;
  font-family: Georgia, serif;
}
h1{
  color: Blue;
}
p {
  color: Teal;
  padding-left: 20px;
}
a{
  color: MidnightBlue;
  text-decoration: none;
}
a:hover {
  color: DarkOrange;
}
```

css and tags should be seen like russian dolls. if `<a>` is inside a `<p>` tag whit itself is inside a `<body>` tag, then all styles defined in the body section of css file apply to p and a while not overwriten. In our example, background-color is not overwriten, then it applies to all elements inside `<body>`. Text color is defined in the p section but it overwriten in the a section, then text color in all <a> sections of the html document is MidnightBlue while text color in p sections is Teal.

Note that we used the syntax `a:hover` that applies to all <a> tag when mouse pointer is over this element. It results in a color change when the mouse points on a link.

When no style is defined like in our previous tries, then the browser styles elements with a standard HTML1.0 ugly design.
