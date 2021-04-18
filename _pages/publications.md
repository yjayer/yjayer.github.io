---
permalink: "/publications/"
layout: home
classes: wide
author_profile: true
title: "Publications"
---

<!-- Books -->
{% capture counter_book %}
  {% bibliography_count -f example --query @book %}
{% endcapture %}
{% if counter_book != "0" %}
  <h2>Books</h2>
  {% bibliography -f example --query @book %}
{% endif %}

<!-- Journal articles-->
{% capture counter_article %}
  {% bibliography_count -f example --query @article %}
{% endcapture %}
{% if counter_article != "0" %}
  <h2>Journal articles</h2>
  {% bibliography -f example --query @article %}
{% endif %}

<!-- Conference papers -->
{% capture counter_inproceedings %}
  {% bibliography_count -f example --query @inproceedings %}
{% endcapture %}
{% if counter_inproceedings != "0" %}
  <h2>Conference papers</h2>
  {% bibliography -f example --query @inproceedings %}
{% endif %}

<!-- Workshop papers -->
{% capture counter_workshop %}
  {% bibliography_count -f example --query @misc[keywords=workshop] %}
{% endcapture %}
{% if counter_workshop != "0" %}
  <h2>Workshop papers</h2>
  {% bibliography -f example --query @misc[keywords=workshop] %}
{% endif %}

<!-- Thesis -->
{% capture counter_thesis %}
  {% bibliography_count -f example --query @thesis %}
{% endcapture %}
{% if counter_thesis != "0" %}
  <h2>Thesis</h2>
  {% bibliography -f example --query @thesis %}
{% endif %}

<!-- Popularization -->
{% capture counter_popularization %}
  {% bibliography_count -f example --query @misc[keywords=popularization] %}
{% endcapture %}
{% if counter_popularization != "0" %}
  <h2>Popularization</h2>
  {% bibliography -f example --query @misc[keywords=popularization] %}
{% endif %}
