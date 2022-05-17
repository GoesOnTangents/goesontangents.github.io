---
title: Leaderboard and Rising Stars
---

# Alternate Uses Task

<table>
  {% for row in site.data.mock_validation %}
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

# Immune Defense

<table>
  {% for row in site.data.aggregated %}
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

# Other Results

Everything can be expressed as a CSV or as just plain text.
This is how plain text looks. 
