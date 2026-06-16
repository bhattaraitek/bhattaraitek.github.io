---
layout: page
title: notes
nav: true
nav_order: 5
permalink: /notes/
---
{% assign notes = site.notes | sort: "title" %}
<ul>
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a></li>
{% endfor %}
</ul>
