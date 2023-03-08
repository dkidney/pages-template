# Make a website with Github pages and R markdown

1. Create a new repo

1. Create an `index.Rmd` file - this will be the website homepage

```
---
title: "Template Github Pages"
author: "Darren Kidney"
date: '`r format(Sys.Date(), "%d %b %Y")`'
output:
    html_document:
        toc: false
---

## title

asdf
```

1. Create a `_site.yml` file

```
name: "name"
output_dir: "."
navbar:
  title: "navbar title"
  left:
    - text: "menu 1"
      menu:
        - text: "basics"
          href: basics.html
  right:
    - text: "how2"
      menu:
        - text: "dkidney"
          href: https://github.com/dkidney
    - icon: fa-github fa-lg
      href: https://github.com/dkidney/pages-template
    - icon: fa-linkedin fa-lg
      href: https://uk.linkedin.com/in/darren-kidney-495b8a103/
```

The Github help docs can be found here, but they don't cover how to set up pages using R Markdown:

https://pages.github.com/

