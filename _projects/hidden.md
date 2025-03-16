---
layout: page
title: Hidden populations
img: assets/img/
importance: 2
category: exclusion 
---

## Project overview

<div class="publications">

  {% bibliography -f projects -q @*[proj~=hidden]* %}

</div>

## Documents

<div class="publications">

  {% bibliography -f papers -q @*[proj~=hidden]* %}

</div>
Pre-analysis plan available at: https://osf.io/pnqmv 
 
    {% assign repo = site.data.repositories.github_repos | where: "url", https://github.com/gerasy1987/hiddenmeta/ | first %}
 {% if repo %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center"> 
    {% include repository/repo.liquid repository=repo %}
  </div>
{% endif %}
