---
layout: page
permalink: /publications/
title: publications
description: ACM CHI and ACM UIST are top conferences for technical HCI work.
years: [2022, 2021, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
