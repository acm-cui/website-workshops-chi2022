---
layout: page
title: Accepted position papers

nav_text: Accepted papers
nav_position: 3
---


The following papers were accepted for inclusion in the workshop (test): 
<!---
<ul>
{% for paper in site.data.papers %}
<li>{% if paper.pdf %}<a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a>{% else %}<strong>{{ paper.title }}</strong>{% endif %}<br>{{ paper.authors }}</li>
{% endfor %}
</ul>
-->
<table>
  <tr>
    <th>Themes</th>
    <th>Author(s)</th>
    <th>Title</th>
  </tr>
  {% for entry in site.data.papers %}
  <tr>
    <td>{{ entry.theme}}</td>
    <td></td>
    <td></td>
  </tr>
  {% for paper in entry.papers %}
  <tr>
    <td></td>
    <td>{{paper.authors}}</td>
    <td><a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a></td>
  </tr>
   {% endfor %}

{% endfor %}
</table>
