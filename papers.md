---
layout: page
title: Accepted position papers

nav_text: Accepted Papers
nav_position: 3
---


The following papers were accepted for inclusion in the workshop: 

<ul>
{% for paper in site.data.papers %}
<li>{% if paper.pdf %}<a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a>{% else %}<strong>{{ paper.title }}</strong>{% endif %}<br>{{ paper.authors }}</li>
{% endfor %}
</ul>
