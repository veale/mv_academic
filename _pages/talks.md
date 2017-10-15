---
layout: page
permalink: /talks/
title: talks
description: Talks by date.
years: [2017, 2016]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}
