---
layout: page
permalink: /publications/
title: publications
description: my publications in reversed chronological order.
years: [2022, 2021, 2020, 2018, 2016, 2014]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
