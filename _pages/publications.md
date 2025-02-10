---
layout: page
permalink: /publications/
title: publications
description:
years: [2025,2024,2023,2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <!-- <h3 class="year">{{y}}</h3> -->
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
