---
title: EPScore23 Benchmark score
layout: page
menu: HS23 scores
---

{% assign row = site.data.HS23scores[0] %}
{% for pair in row %}
  {{ pair | inspect }}
{% endfor %}