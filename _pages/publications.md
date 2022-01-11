---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order. You can also find my articles on <a href='https://scholar.google.com/citations?user=51itJEEAAAAJ&hl=en/'>my Google Scholar profile</a>. 
years: [2021,2020,2019,2018,2017,2016]
nav: true
---
TOP 4 Security Conferences (S&P, CCS, USENIX, NDSS)

TOP 4 Software Engineering (ICSE, FSE, ASE, ISSTA)

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
