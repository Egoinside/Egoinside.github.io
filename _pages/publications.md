---
layout: page
permalink: /publications/
title: publications
description: 
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