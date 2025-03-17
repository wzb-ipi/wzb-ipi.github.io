---
layout: page
permalink: /writing/by_year/
title: by year
description:   
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: false
---

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

