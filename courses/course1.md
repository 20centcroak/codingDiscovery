---
layout: course
title: My first html page
number: 1
---

 html is a computer language. It is composed of tags like that: `<html>` and text.
 Afterwards this language is understood and displayed by internet browser.

 Try this most simple example, create a *index.html* file and copy paste this inside:
```html
<html>
  Hello world
</html>
```

Then open this file in your internet browser and you will see your message! As you can see, tags are not displayed, they are only used by the internet browser to understand the content of the file and how to display it. Tags are most generaly pairs that are open and closed: `<html></html>`

Even if this simple example works, this is thanks to the fact that internet browsers are very permissive. But if we want to have no surprise about how text will be displayed, we should add more details to explicitely describe the content of our file.

Here is a second example:
```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>My first html page</title>
  </head>
  <body>
    Hello world!
  </body>
</html>
```

This is a best formed html file. It gives exactly the same result but we can see more tags:
- `<!DOCTYPE html>`:  define which version of html is used in this file. Here we define that we use HTML5 version
- in `<html>` tag, we define the language: `lang="en"`. *en* means english, *fr* for french. We also define the text direction: `dir="ltr"`. *ltr* means left to right.
- we introduce the `<head>` tag pair. Inside, we can add more details about our document. For example adding a title to our file that will be displayed by the browser in its title bar or in the tab name as shown in the figure below:  

![page with title]({{ page.githubRepo}}/assets/images/htmlpart1Title.png)

- then the part to be displayed is inside the `<body>` tag pair.

As all of this soup has to be redone for each html page we build, a more convenient way to add a well formated file is to use a template such as the [html5 boilerplate](https://html5boilerplate.com). Anotther way is to use IDE. This means a specific piece of software to work on software development. For example [Atom](https://atom.io/) or [Visual Studio Code](https://code.visualstudio.com) help saving a lot of time when building a website.

We will see other way to focus only on the content we want to display and not on this soup.
