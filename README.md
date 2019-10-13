# Coding Discovery
This is a journey to discover how informatics work and how to build something with coding languages. It does not go deep into a specific language but list useful links to go farther and give all good practices used in the industry. The website is available here: https://20centcroak.github.io/codingDiscovery/.


## Behind the scene
Behind the scene, this courses make use of github pages and Jekyll. The project structure may be use to build any other static website with a navbar composed of the list of courses, and a 3-tab layout to expose course/handson/result.

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

All *fr* folders concern french articles, and all *en* folders are their english translations. The number variable used in all documents link courses with handsons and results. For example, if course number is 1, and if handsons number 1 exist, it will be displayed in the handson tab associated with course 1. If result number 1 does not exist, the result tabl won't be displayed.

If we want to insert a course between course 1 and course 2, then a course number 1.1 is possible. It avoids changing anything in existing courses and structure. 

To work offline and preview the Jekyll rendering locally, install Jekyll using this [guide](https://jekyllrb.com/docs/installation/). Then add the following content to the gemfile (in the root folder) 
```
# frozen_string_literal: true
source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"
gem "jekyll"
gem "github-pages", group: :jekyll_plugins

gem 'wdm', '>= 0.1.0' if Gem.win_platform?
```

Open a command line in the root folder and execute this line to build the pages and run a local server. With this command line, any modification of the files will induce a re-build by Jekyll:
```
bundle exec jekyll serve
```

update your dependencies regularaly by using:
```
bundle update
```

I you are using git to commit and push your local files to a remote repo, add a .gitignore file with the following content before your first commit:
```
_site/
.sass-cache/
.jekyll-cache/
.jekyll-metadata
```
