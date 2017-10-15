---
layout: page
permalink: /publications/
title: publications
description: Publications by year. Open access indicated by <i class="ai ai-open-access"></i>.
years: [2017, 2016, 2015]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f personal_bibliography -q @*[year={{y}}]* %}
{% endfor %}
