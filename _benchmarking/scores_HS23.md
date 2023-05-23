---
title: EPScore23 Benchmark score
layout: page
menu: HS23 scores
---


<table>
  {% for row in site.data.HS23scores.csv %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>