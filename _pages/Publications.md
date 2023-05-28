---
layout: page
permalink: /Publications/
title: Publications
description: 
years: [2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/Publications.md -->
<div class="Publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
