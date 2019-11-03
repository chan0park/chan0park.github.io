---
layout: page
permalink: /publications/
title: publications
description: 
years: [2019]
---

{% for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
