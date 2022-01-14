---
layout: page
permalink: /publications/
title: publications
description: (* indicates equal contribution)
years: [2022,2021,2020,2019]
---

{% for y in page.years %}
  <h4><b>{{y}}</b></h4>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
