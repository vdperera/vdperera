---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2020, 2018, 2017, 2016, 2015, 2013, 2012]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
