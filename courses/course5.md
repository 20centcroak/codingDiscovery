---
layout: course
title: To go farther...
number: 5
---

You have seen, it does not look so hard to create a webpage. However, if you want a design that fits what you have in mind and that will be displayed nicely on any internet brower and any screen size (mobile, tablet, computer, tv), things are not so obvious. Anyway you can do it, with the help of different websites such as:
- [w3schools](https://www.w3schools.com/)
- [alsacreations](https://www.alsacreations.com/)
- [codecademy](https://www.codecademy.com/learn/learn-html)
- [open classrooms](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3) (French)
- [mozilla](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [freecodecamp](https://www.freecodecamp.org/news/learn-responsive-web-design-in-5-minutes/)

But what if you don't have to bother with the technology and could focus on content? This is what offers a framework ([what's this](https://en.wikipedia.org/wiki/Software_framework)) like [Bootstrap](https://getbootstrap.com/).

Just think: what if in my example about links, and with no more effort, I could achieve a more modern and less ugly result than undelined blue links?

Let see how we can do that with bootstrap:
```
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>styling with bootstrap</title>
    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
  </head>
  <body>
    <a href="https://github.com/20centcroak/childrencourses">visit children courses</a>
    <a href="sample1.html">see sample1</a>
    <a href="https://github.com/20centcroak/childrencourses" target="_blank">visit children courses in a separate tag</a>
  </body>
</html>
```

We have just added the line
```
<!-- Bootstrap CSS -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```
in the head section. Note that `<!-- Bootstrap CSS -->` is a comment and won't never be deisplayed or read by the brower.
The line `<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">` associates a default css file defined by bootstrap and then you can take benefit from a standard style.

Now let see the basic html page defined by bootstrap to display "Hello World":
```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
  </body>
</html>
```

We can see new tags:
- `<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">` will allow the design for different screen sizes
- `<script src=...>` define scripts (=computer programs) to be executed when the page is displayed.

Bootstrap offers tools and technological elements to build easily a website taking into account all the mess about screens and browsers. The large collection of elements is well documenting with examples, go and see this example :
[bootstrap component (carousel)](https://getbootstrap.com/docs/4.3/components/carousel/)
