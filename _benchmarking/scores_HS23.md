---
title: EPScore23 Benchmark score
layout: page
menu: HS23 scores
---

 {% assign table_rows = site.data.HS23scores %}

<br>

<div id="my-table" class="datatable-begin">

  <table>
      {% for row in table_rows %}
          {% if forloop.first %}
              <tr>
                  {% for pair in row %}
                      <th>
                          {{ pair[0] }}
                      </th>
                  {% endfor %}
              </tr>
          {% endif %}

          {% tablerow pair in row %}
              {{ pair[1] }}
          {% endtablerow %}
      {% endfor %}
  </table>

<div class="datatable-end"></div>