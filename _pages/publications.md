---
layout: page
permalink: /publications/
title: publications
description: 
years: [2022]
nav: true
nav_order: 3
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
