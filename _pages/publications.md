---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2025, 2024, 2022]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

<div class="publications">

{%- for y in page.years %}

  <h2 class="year">{{y}}</h2>

  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>