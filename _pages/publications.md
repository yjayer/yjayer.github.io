---
permalink: "/publications/"
layout: home
author_profile: true
title: "Publications"
classes: wide
---

You can also have a look at
<a href="https://scholar.google.com"><i class="ai ai-google-scholar" aria-hidden="true"></i>Scholar</a>

### Books

  {% bibliography -f example --query @book %}

### Journal papers

  {% bibliography -f example --query @article %}

### Conference papers

  {% bibliography -f example --query @inproceedings %}

### Workshop papers

  {% bibliography -f example --query @misc[keywords=workshop] %}

### Thesis

  {% bibliography -f example --query @thesis %}

### Popularization

  {% bibliography -f example --query @misc[keywords=popularization] %}
