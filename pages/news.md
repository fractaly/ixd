---
layout: default
published: true
permalink: /news/
title: News
color: '#000'
order: 0
---

wowowowow
{% for n in site.news  reversed %}
<article>
  <h4> {{ n.title }} </h4>
  <date>{{ n.date | date: '%B %d, %Y' }}</date>
  {{ n.content }}
</article>
{% endfor %}
