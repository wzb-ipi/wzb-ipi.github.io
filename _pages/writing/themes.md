---
layout: page
permalink: /themes/
title: by theme
description:   
keywords: [vertical linkages, horizontal contestation, exclusion, elite connections, methods]
nav: false
---


<!-- _pages/publications.md -->
<div class="publications">

{%- for x in page.keywords %}
  <h2 class="key" id = {{x}}>{{x}}</h2>
  {% bibliography -f papers -q @*[keywords~={{ x }}]* %}
{% endfor %}

</div>


---
