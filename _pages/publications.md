---
layout: page
permalink: /publications/
title: Publications
description: Please see my <a href='https://scholar.google.com/citations?user=GuKEDfixZqsC&hl=en'>google scholar</a> for a full list of publications
years: [2021,2020,2019]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
