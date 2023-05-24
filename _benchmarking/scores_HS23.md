---
title: EPScore23 Benchmark score
layout: page
menu: HS23 scores
datatable: true
---

 {% assign table_rows = site.data.HS23scores %}

<br>
table

  <table class="display">
      {% for row in table_rows %}
          {% if forloop.first %}
              <thead>
              <tr>
                  {% for pair in row %}
                      <th>
                          {{ pair[0] }}
                      </th>
                  {% endfor %}
              </tr>
              </thead>
          {% endif %}

          {% tablerow pair in row %}
              {{ pair[1] }}
          {% endtablerow %}
      {% endfor %}
  </table>

