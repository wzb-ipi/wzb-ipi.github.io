---
layout: page
permalink: /publications/
title: publications
description: ipi publications by year
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017]
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

---
---
layout: page
permalink: /publications/
title: publications
description: IPI publications by topical area
keywords: [vertical linkages, horizontal contestation, exclusion, elite connections, methods]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">

{%- for keywords in page.keywords %}
  <h2 class="keywords">{{ keywords }}</h2>
  {% bibliography -f papers -q @*[keywords~={{ keywords }}]* %}
{% endfor %}

</div>
---
