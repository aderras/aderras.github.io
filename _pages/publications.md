---
layout: page
permalink: /publications/
title: publications
description: 
years:  [2018,2019,2021,2022,2024]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years reversed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
