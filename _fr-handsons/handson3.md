---
layout: course-fr
title: Make it pretty
number: 3
---

1. add in your previous html page the following line between `<head>` tags
```
    <link rel="stylesheet" href="css/styles.css">
```
1. add tags like `<h1>, <h2>, ...` for titles and `<p>` for paragraphs and add text between these tags, for example:
```
<h1>This is my title</h1>
```

1. Create a a file named *styles.css* and save it in a folder called *css* located at the same place than your html file

1. define styles for the tags you added. You can use properties like `background-color` or `color` with a color name (you can pick one in the list given [here](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)).

1. open the file in your browser and see if the result is as expected.

1. create another *styles2.css* in the *css* folder
1. define different styles in this file.
1. let your html file point on this new file by changing this line:
```
    <link rel="stylesheet" href="css/styles2.css">
```
1. refresh your browser (F5) and see that your page looks different thanks to this only change to the css file reference.

see [sample4](../htmlpart1/sample4.html) and [styles](../htmlpart1/css/styles.css) for help.
