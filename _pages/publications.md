---
layout: publication
permalink: /publications/
title: publication
description: publications by categories in reversed chronological order. generated by jekyll-scholar.
years: [1905, 1935, 1950, 1956]
nav: true

search:
  align: left
---

<div class="publications">

<ul>
{% for y in page.years %}
<li>  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
</li>
{% endfor %}
</ul>

</div>
