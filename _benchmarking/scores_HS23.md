---
title: EPScore23 Benchmark score
layout: page
menu: HS23 scores
---

<table>
  {% for row in site.data.HS23scores %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[1] }}</th>
      {% endfor %}
    </tr>
    {% endif %}


  {% endfor %}
</table>