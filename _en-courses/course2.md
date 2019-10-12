---
layout: course-en
title: Linking pages
number: 2
---

 What is the most interesting feature in HTML is the link to other html pages or to other sections of the same page.

 For example, if you want the reader to be able to click and go to qwant, just add the link to qwant, called *url* in a `<a>` tag like this:
 ```
 <a href="https://github.com/20centcroak/childrencourses">visit children courses</a>
 ```

If you would like to direct to another of your pages, indicate a *relative link*:
```
<a href="sample1.html">see sample1</a>
```

It is also possible to open this link in another tag, using the *target* keyword in the *<a>* tag:
```
 <a href="https://github.com/20centcroak/childrencourses" target="_blank">children courses</a>
```
