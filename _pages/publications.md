---
layout: page
permalink: /publications/
title: publications
description: [[Google Scholar]](https://scholar.google.com/citations?hl=zh-CN&user=hr2JciwAAAAJ)
years: []
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">




{% bibliography -f papers %}


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}



</div>