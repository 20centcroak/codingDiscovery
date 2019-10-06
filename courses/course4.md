---
layout: course
title: Animations
number: 4
---

We will see that it is possible to use css to make small animations, which is quite funny.
But before, we should introduce some useful new tags and properties.

# div and class

First, welcome the `<div>` tag. This tag is the most used one when building a webpage. It separates sections or blocks in this page. For example if you want to display a naivigation bar, a footer, or some columns, you wil use `<div>`

Secondly, applaude the class property that could be apply to any tag like this:
```
<div class="section1">this is section 1</div>
<div class = "section2">
  <h1>Section2 title</h1>
  <p class="section2Paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
</div>
```

([what is this strange *Lorem ipsum...* text?](https://lipsum.com/))

With this class, we can now add style not only to tags but also to class. Then for example, all the `<div>, <h1>, <p>` tags can look differently if they are associated with a class that has a specific styling.

Here is an example of the asscociated css file:
```
.section1{
  background-color: DarkGreen;
}
.section2{
  background-color: Blue;
}
.section2Paragraph{
  background-color: Cyan;
}
```

# Css animations
Well, now a piece of fun! Let see css animations.

Animations can be declared in css file like this:
```
.move {
  width: 100px;
  height: 100px;
  background-color: navy;
  position: relative;
  animation-name: my-animation;
  animation-duration: 4s;
  border-radius: 50px;
}

/* Standard syntax */
@keyframes my-animation {
  0%   {background-color:navy; left:0px; top:0px;}
  25%  {background-color:blue; left:100px; top:50px;}
  50%  {background-color:teal; left:50px; top:150px;}
  75%  {background-color:purple; left:50px; top:50px;}
  100% {background-color:deeppink; left:0px; top:0px;}
}
```
In the move class definition, we define the dimensions of the element, the background-color, a border-radius that will result in a circle shape, and the following animation properties:
- animation-name: this will be used by the next css definition starting with @keyframes
- animation-duration: it defines the time of this animation.

Then the animation itself is defined in the @keyframes element. This is the sequence to be executed during the given 4s duration. We should declare the name of the animation for which this execution applies (here: *my-animation*). This sequence says :
- during the 25% of time (=1s), background color will vary from navy to blue and the shape will be moved 100px right and 50px bottom (as you can see we declare left and top, not right and bottom, this is because we simply add a margin left and top which results in a shape deplacement to right and bottom)
- from 25% to 50% of the animation (the next 1s of the animation), background will vary from blue to teal and will be moved 50px left and 50px bottom.
- and so on...
