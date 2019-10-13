# Coding Discovery
This is a journey to discover how informatics work and how to code your very first programs.

This courses make use of github pages and Jekyll. The project structure may be use to build any other static website with a navbar composed of the list of courses, and a 3-tab layout to expose course/handson/result.

Basically, the collections for courses, handsons and results are declare in the `_config.yml` file like this:
```
collections:
  en-courses:
    sort_by: number
    output: true
    permalink: /:collection/:name

  en-handsons:
    sort_by: number
    output: true
    permalink: /:collection/:name

  en-results:
    sort_by: number
    output: true
    permalink: /:collection/:name

  fr-courses:
    sort_by: number
    output: true
    permalink: /:collection/:name

  fr-handsons:
    sort_by: number
    output: true
    permalink: /:collection/:name

  fr-results:
    sort_by: number
    output: true
    permalink: /:collection/:name
```

Then, according to Jekyll structure, the following folders should be created at the root of the website:
- _fr-courses
- _fr-handsons
- _fr-results
- _en-courses
- _en-handsons
- _en-results

All *fr* folders concern french articles, and all *en* folders are their english translations.
