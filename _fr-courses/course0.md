---
layout: course-fr
title: Table des matières
number: 0
---

{% for course in site.fr-courses %}
  {% if getNext %}{% assign next = course.url %}{% assign getNext = false %}{% endif %}
  {% if course.number == page.number %}{% assign getNext = true %}{% continue %}{% endif %}
  - [{{ course.title }}]({{ course.url | relative_url }})
{% endfor %}
