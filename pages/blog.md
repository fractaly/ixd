---
layout: default
published: true
permalink: /projects/
title: Projects
color: "#000"
order: 1
---

{% for n in site.projects  reversed %}
<article>
  <h4> {{ n.title }} </h4>
  <date>{{ n.date | date: '%B %d, %Y' }}</date>
  {{ n.content }}
</article>
{% endfor %}

