---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order. You can also find my articles on [my Google Scholar profile](https://scholar.google.com/citations?user=51itJEEAAAAJ&hl=en).
years: [2021,2020,2019,2018,2017]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
